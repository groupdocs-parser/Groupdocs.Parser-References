---
title: Parser
second_title: .NET API 참조용 GroupDocs.Parser
description: 의 새 인스턴스를 초기화합니다.Parsergroupdocs.parser/parser 데이터베이스에서 데이터를 추출하는 클래스.
type: docs
weight: 10
url: /ko/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 데이터베이스에서 데이터를 추출하는 클래스.

```csharp
public Parser(DbConnection connection)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| connection | DbConnection | 데이터베이스 연결입니다. |

### 비고

**더 알아보기:**

* [데이터베이스에서 데이터 추출](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### 예

다음 예는 Sqlite 데이터베이스에서 데이터를 추출하는 방법을 보여줍니다.

```csharp
// DbConnection 객체 생성
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 데이터베이스에서 테이블을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다.
using (Parser parser = new Parser(connection))
{
    // 텍스트 추출 지원 여부 확인
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // toc 추출 지원 여부 확인
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 테이블 목록 가져오기
    IEnumerable<TocItem> toc = parser.GetToc();
    // 테이블 반복
    foreach (TocItem i in toc)
    {
        // 테이블 이름 출력
        Console.WriteLine(i.Text);
        // 테이블 내용을 텍스트로 추출
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 또한보십시오

* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 데이터베이스에서 데이터를 추출하는 클래스.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| connection | DbConnection | 데이터베이스 연결입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 지정하는 데 사용되는 파서 설정입니다. |

### 비고

**더 알아보기:**

* [데이터베이스에서 데이터 추출](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [벌채 반출](https://docs.groupdocs.com/display/parsernet/Logging)

### 예

다음 예는 Sqlite 데이터베이스에서 데이터를 추출하는 방법을 보여줍니다.

```csharp
// DbConnection 객체 생성
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 데이터베이스에서 테이블을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다.
using (Parser parser = new Parser(connection))
{
    // 텍스트 추출 지원 여부 확인
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // toc 추출 지원 여부 확인
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 테이블 목록 가져오기
    IEnumerable<TocItem> toc = parser.GetToc();
    // 테이블 반복
    foreach (TocItem i in toc)
    {
        // 테이블 이름 출력
        Console.WriteLine(i.Text);
        // 테이블 내용을 텍스트로 추출
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 또한보십시오

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 원격 이메일 서버에서 데이터를 추출하는 클래스.

```csharp
public Parser(EmailConnection connection)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| connection | EmailConnection | 이메일 연결입니다. |

### 비고

**더 알아보기:**

* [POP, IMAP 또는 Exchange 웹 서비스 프로토콜을 통해 원격 서버에서 이메일 추출](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### 예

다음 예는 Exchange Server에서 이메일을 추출하는 방법을 보여줍니다.

```csharp
// Exchange 웹 서비스 프로토콜에 대한 연결 객체 생성 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// 원격 서버에서 이메일을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다.
using (Parser parser = new Parser(connection))
{
    // 컨테이너 추출 지원 여부 확인
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// 서버에서 이메일 메시지 추출
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 첨부 파일을 반복합니다.
    foreach (ContainerItem item in emails)
    {
        // 이메일 메시지에 대한 Parser 클래스의 인스턴스 생성
        using (Parser emailParser = item.OpenParser())
        {
            // 이메일 텍스트 추출
            using (TextReader reader = emailParser.GetText())
            {
                // 이메일 텍스트 출력
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 또한보십시오

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 원격 이메일 서버에서 데이터를 추출하는 클래스.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| connection | EmailConnection | 이메일 연결입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 지정하는 데 사용되는 파서 설정입니다. |

### 비고

**더 알아보기:**

* [POP, IMAP 또는 Exchange 웹 서비스 프로토콜을 통해 원격 서버에서 이메일 추출](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [벌채 반출](https://docs.groupdocs.com/display/parsernet/Logging)

### 예

다음 예는 Exchange Server에서 이메일을 추출하는 방법을 보여줍니다.

```csharp
// Exchange 웹 서비스 프로토콜에 대한 연결 객체 생성 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// 원격 서버에서 이메일을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다.
using (Parser parser = new Parser(connection))
{
    // 컨테이너 추출 지원 여부 확인
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// 서버에서 이메일 메시지 추출
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 첨부 파일을 반복합니다.
    foreach (ContainerItem item in emails)
    {
        // 이메일 메시지에 대한 Parser 클래스의 인스턴스 생성
        using (Parser emailParser = item.OpenParser())
        {
            // 이메일 텍스트 추출
            using (TextReader reader = emailParser.GetText())
            {
                // 이메일 텍스트 출력
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 또한보십시오

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 클래스.

```csharp
public Parser(string filePath)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일의 경로입니다. |

### 비고

**더 알아보기:**

* [로컬 디스크에서 문서 로드](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 예

다음 예에서는 로컬 디스크에서 문서를 로드하는 방법을 보여줍니다.

```csharp
// filePath를 사용하여 Parser 클래스의 인스턴스를 생성합니다.
using (Parser parser = new Parser(filePath))
{
    // 리더에 텍스트 추출
    using (TextReader reader = parser.GetText())
    {
        // 문서에서 텍스트 출력
        // 텍스트 추출이 지원되지 않는 경우 판독기는 null입니다.
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 또한보십시오

* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 와 수업[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일의 경로입니다. |
| loadOptions | LoadOptions | 파일을 여는 옵션입니다. |

### 비고

**더 알아보기:**

* [특정 파일 형식 로드](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [암호로 보호된 문서 로드](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [로컬 디스크에서 문서 로드](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 예

문서 암호는 LoadOptions 클래스에 의해 전달됩니다.

```csharp
try
{
    // 암호를 사용하여 Parser 클래스의 인스턴스를 만듭니다.
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // 텍스트 추출 지원 여부 확인
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트 출력
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // 비밀번호가 틀리거나 비어있는 경우 메시지 출력
    Console.WriteLine("Invalid password");
}
```

### 또한보십시오

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 와 수업[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일의 경로입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 지정하는 데 사용되는 파서 설정입니다. |

### 또한보십시오

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 와 수업[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 및[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일의 경로입니다. |
| loadOptions | LoadOptions | 파일을 여는 옵션입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 지정하는 데 사용되는 파서 설정입니다. |

### 비고

**더 알아보기:**

* [특정 파일 형식 로드](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [암호로 보호된 문서 로드](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [벌채 반출](https://docs.groupdocs.com/display/parsernet/Logging)
* [로컬 디스크에서 문서 로드](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 예

다음 예는 다음을 통해 정보를 수신하는 방법을 보여줍니다.[`ILogger`](../../../groupdocs.parser.options/ilogger) 상호 작용:

```csharp
// 노력하다
{
    // Logger 클래스의 인스턴스 생성
    Logger logger = new Logger();
    // 파서 설정으로 Parser 클래스의 인스턴스 생성
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // 텍스트 추출 지원 여부 확인
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트 출력
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // 예외 무시
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // 오류 메시지 출력
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // 이벤트 메시지 출력
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 경고 메시지 출력
        Console.WriteLine("Warning: " + message);
    }
}
```

### 또한보십시오

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 클래스.

```csharp
public Parser(Stream document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| document | Stream | 소스 입력 스트림입니다. |

### 비고

**더 알아보기:**

* [스트림에서 문서 로드](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 예

다음 예에서는 스트림에서 문서를 로드하는 방법을 보여줍니다.

```csharp
// 스트림을 사용하여 Parser 클래스의 인스턴스를 만듭니다.
using (Parser parser = new Parser(stream))
{
    // 리더에 텍스트 추출
    using (TextReader reader = parser.GetText())
    {
        // 문서에서 텍스트 출력
        // 텍스트 추출이 지원되지 않는 경우 판독기는 null입니다.
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 또한보십시오

* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 와 수업[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| document | Stream | 소스 입력 스트림입니다. |
| loadOptions | LoadOptions | 파일을 여는 옵션입니다. |

### 비고

**더 알아보기:**

* [특정 파일 형식 로드](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [암호로 보호된 문서 로드](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [스트림에서 문서 로드](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 예

경우에 따라 정의해야 합니다.[`FileFormat`](../../../groupdocs.parser.options/fileformat). 특수한 경우(데이터베이스, 이메일 서버) 및 내용으로 파일 유형 감지:

문서 암호가 전달됩니다.[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 수업:

```csharp
// 마크다운 문서용 Parser 클래스 인스턴스 생성
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // 텍스트 추출 지원 여부 확인
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // 문서 텍스트 출력
        // 마크다운이 감지되었습니다. 특수 기호가 없는 텍스트가 인쇄됩니다.
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // 암호를 사용하여 Parser 클래스의 인스턴스를 만듭니다.
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // 텍스트 추출 지원 여부 확인
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트 출력
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // 비밀번호가 틀리거나 비어있는 경우 메시지 출력
    Console.WriteLine("Invalid password");
}
```

### 또한보십시오

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 와 수업[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| document | Stream | 소스 입력 스트림입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 지정하는 데 사용되는 파서 설정입니다. |

### 또한보십시오

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

의 새 인스턴스를 초기화합니다.[`Parser`](../../parser) 와 수업[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 및[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| document | Stream | 소스 입력 스트림입니다. |
| loadOptions | LoadOptions | 파일을 여는 옵션입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 지정하는 데 사용되는 파서 설정입니다. |

### 비고

**더 알아보기:**

* [특정 파일 형식 로드](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [암호로 보호된 문서 로드](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [스트림에서 문서 로드](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [벌채 반출](https://docs.groupdocs.com/display/parsernet/Logging)

### 예

다음 예는 다음을 통해 정보를 수신하는 방법을 보여줍니다.[`ILogger`](../../../groupdocs.parser.options/ilogger) 상호 작용:

```csharp
// 노력하다
{
    // Logger 클래스의 인스턴스 생성
    Logger logger = new Logger();
    // 파서 설정으로 Parser 클래스의 인스턴스 생성
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // 텍스트 추출 지원 여부 확인
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트 출력
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // 예외 무시
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // 오류 메시지 출력
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // 이벤트 메시지 출력
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 경고 메시지 출력
        Console.WriteLine("Warning: " + message);
    }
}
```

### 또한보십시오

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
