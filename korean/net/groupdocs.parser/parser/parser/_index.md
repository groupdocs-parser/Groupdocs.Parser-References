---
title: "파서"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "URI에서 데이터를 추출하기 위해 Parsergroupdocs.parser/parser 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

URI에서 데이터를 추출하기 위해 [`Parser`](../../parser) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Parser(Uri uri)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uri | Uri | 요청이 전송되는 Uri. |

### 참고

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 URI에서 *loadOptions* 로 데이터를 추출합니다.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uri | Uri | 요청이 전송되는 Uri. |
| loadOptions | LoadOptions | 파일을 열기 위한 옵션입니다. |

### 참고

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 URI에서 *parserSettings* 로 데이터를 추출합니다.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uri | Uri | 요청이 전송되는 Uri. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 참고

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 URI에서 *loadOptions* 및 *parserSettings* 로 데이터를 추출합니다.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uri | Uri | 요청이 전송되는 Uri. |
| loadOptions | LoadOptions | 파일을 열기 위한 옵션입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 참고

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 데이터베이스에서 데이터를 추출합니다.

```csharp
public Parser(DbConnection connection)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 연결 | DbConnection | 데이터베이스 연결입니다. |

### 비고

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### 예제

다음 예제는 Sqlite 데이터베이스에서 데이터를 추출하는 방법을 보여줍니다:

```csharp
// DbConnection 객체 생성
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 데이터베이스에서 테이블을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(connection))
{
    // 텍스트 추출이 지원되는지 확인합니다
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 목차 추출이 지원되는지 확인합니다
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 테이블 목록 가져오기
    IEnumerable<TocItem> toc = parser.GetToc();
    // 테이블을 반복합니다
    foreach (TocItem i in toc)
    {
        // 테이블 이름 출력
        Console.WriteLine(i.Text);
        // 테이블 내용을 텍스트로 추출합니다
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 참고

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 데이터베이스에서 데이터를 추출합니다.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 연결 | DbConnection | 데이터베이스 연결입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 비고

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 예제

다음 예제는 Sqlite 데이터베이스에서 데이터를 추출하는 방법을 보여줍니다:

```csharp
// DbConnection 객체 생성
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 데이터베이스에서 테이블을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(connection))
{
    // 텍스트 추출이 지원되는지 확인합니다
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 목차 추출이 지원되는지 확인합니다
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 테이블 목록 가져오기
    IEnumerable<TocItem> toc = parser.GetToc();
    // 테이블을 반복합니다
    foreach (TocItem i in toc)
    {
        // 테이블 이름 출력
        Console.WriteLine(i.Text);
        // 테이블 내용을 텍스트로 추출합니다
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 참고

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 원격 이메일 서버에서 데이터를 추출합니다.

```csharp
public Parser(EmailConnection connection)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 연결 | EmailConnection | 이메일 연결입니다. |

### 비고

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### 예제

다음 예제는 Exchange Server에서 이메일을 추출하는 방법을 보여줍니다:

```csharp
// Exchange Web Services 프로토콜용 연결 객체 생성
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// 원격 서버에서 이메일을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(connection))
{
    // 컨테이너 추출이 지원되는지 확인합니다
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// 서버에서 이메일 메시지를 추출합니다
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 첨부 파일을 반복합니다
    foreach (ContainerItem item in emails)
    {
        // 이메일 메시지를 위해 Parser 클래스의 인스턴스를 생성합니다
        using (Parser emailParser = item.OpenParser())
        {
            // 이메일 텍스트를 추출합니다
            using (TextReader reader = emailParser.GetText())
            {
                // 이메일 텍스트를 출력합니다
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 참고

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화하여 원격 이메일 서버에서 데이터를 추출합니다.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 연결 | EmailConnection | 이메일 연결입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 비고

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 예제

다음 예제는 Exchange Server에서 이메일을 추출하는 방법을 보여줍니다:

```csharp
// Exchange Web Services 프로토콜용 연결 객체 생성
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// 원격 서버에서 이메일을 추출하기 위해 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(connection))
{
    // 컨테이너 추출이 지원되는지 확인합니다
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// 서버에서 이메일 메시지를 추출합니다
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 첨부 파일을 반복합니다
    foreach (ContainerItem item in emails)
    {
        // 이메일 메시지를 위해 Parser 클래스의 인스턴스를 생성합니다
        using (Parser emailParser = item.OpenParser())
        {
            // 이메일 텍스트를 추출합니다
            using (TextReader reader = emailParser.GetText())
            {
                // 이메일 텍스트를 출력합니다
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 참고

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Parser(string filePath)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| filePath | 문자열 | 파일 경로입니다. |

### 비고

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 예제

다음 예제는 로컬 디스크에서 문서를 로드하는 방법을 보여줍니다:

```csharp
// filePath를 사용하여 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 텍스트를 리더에 추출
    using (TextReader reader = parser.GetText())
    {
        // 문서에서 텍스트를 출력합니다
        // 텍스트 추출이 지원되지 않으면, 리더는 null입니다
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 참고

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

`[`Parser`](../../parser)` 클래스의 새 인스턴스를 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions)와 함께 초기화합니다.

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| filePath | 문자열 | 파일 경로입니다. |
| loadOptions | LoadOptions | 파일을 열기 위한 옵션입니다. |

### 비고

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 예제

문서 비밀번호는 LoadOptions 클래스에 의해 전달됩니다:

```csharp
try
{
    // 비밀번호를 사용하여 Parser 클래스의 인스턴스를 생성합니다:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // 텍스트 추출이 지원되는지 확인합니다
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트를 출력합니다
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // 비밀번호가 올바르지 않거나 비어 있을 경우 메시지를 출력합니다
    Console.WriteLine("Invalid password");
}
```

### 참고

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

`[`Parser`](../../parser)` 클래스의 새 인스턴스를 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings)와 함께 초기화합니다.

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| filePath | 문자열 | 파일 경로입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 참고

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

`[`Parser`](../../parser)` 클래스의 새 인스턴스를 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions)와 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings)와 함께 초기화합니다.

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| filePath | 문자열 | 파일 경로입니다. |
| loadOptions | LoadOptions | 파일을 열기 위한 옵션입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 비고

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 예제

다음 예제는 [`ILogger`](../../../groupdocs.parser.options/ilogger) 인터페이스를 통해 정보를 받는 방법을 보여줍니다:

```csharp
// try
{
    // Logger 클래스의 인스턴스를 생성합니다
    Logger logger = new Logger();
    // parser settings를 사용하여 Parser 클래스의 인스턴스를 생성합니다
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // 텍스트 추출이 지원되는지 확인합니다
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트를 출력합니다
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // 오류 메시지를 출력합니다
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // 이벤트 메시지를 출력합니다
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 경고 메시지를 출력합니다
        Console.WriteLine("Warning: " + message);
    }
}
```

### 참고

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

[`Parser`](../../parser) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Parser(Stream document)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 문서 | Stream | 소스 입력 스트림입니다. |

### 비고

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 예제

다음 예제는 스트림에서 문서를 로드하는 방법을 보여줍니다:

```csharp
// 스트림을 사용하여 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(stream))
{
    // 텍스트를 리더에 추출
    using (TextReader reader = parser.GetText())
    {
        // 문서에서 텍스트를 출력합니다
        // 텍스트 추출이 지원되지 않으면, 리더는 null입니다
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 참고

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

`[`Parser`](../../parser)` 클래스의 새 인스턴스를 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions)와 함께 초기화합니다.

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 문서 | Stream | 소스 입력 스트림입니다. |
| loadOptions | LoadOptions | 파일을 열기 위한 옵션입니다. |

### 비고

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 예제

일부 경우에는 [`FileFormat`](../../../groupdocs.parser.options/fileformat)을 정의해야 합니다. 특수한 경우(데이터베이스, 이메일 서버)와 콘텐츠를 통해 파일 유형을 감지하는 경우 모두에 해당합니다:

```csharp
// markdown 문서를 위해 Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // 텍스트 추출이 지원되는지 확인합니다
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // 문서 텍스트를 출력합니다
        // Markdown이 감지되었습니다; 특수 기호가 없는 텍스트가 출력됩니다
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

문서 비밀번호는 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 클래스에 의해 전달됩니다:

```csharp
try
{
    // 비밀번호를 사용하여 Parser 클래스의 인스턴스를 생성합니다:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // 텍스트 추출이 지원되는지 확인합니다
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트를 출력합니다
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // 비밀번호가 올바르지 않거나 비어 있을 경우 메시지를 출력합니다
    Console.WriteLine("Invalid password");
}
```

### 참고

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

`[`Parser`](../../parser)` 클래스의 새 인스턴스를 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings)와 함께 초기화합니다.

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 문서 | Stream | 소스 입력 스트림입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 참고

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

`[`Parser`](../../parser)` 클래스의 새 인스턴스를 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions)와 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings)와 함께 초기화합니다.

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 문서 | Stream | 소스 입력 스트림입니다. |
| loadOptions | LoadOptions | 파일을 열기 위한 옵션입니다. |
| parserSettings | ParserSettings | 데이터 추출을 사용자 정의하는 데 사용되는 파서 설정입니다. |

### 비고

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 예제

다음 예제는 [`ILogger`](../../../groupdocs.parser.options/ilogger) 인터페이스를 통해 정보를 받는 방법을 보여줍니다:

```csharp
// try
{
    // Logger 클래스의 인스턴스를 생성합니다
    Logger logger = new Logger();
    // parser settings를 사용하여 Parser 클래스의 인스턴스를 생성합니다
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // 텍스트 추출이 지원되는지 확인합니다
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 문서 텍스트를 출력합니다
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // 오류 메시지를 출력합니다
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // 이벤트 메시지를 출력합니다
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 경고 메시지를 출력합니다
        Console.WriteLine("Warning: " + message);
    }
}
```

### 참고

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
