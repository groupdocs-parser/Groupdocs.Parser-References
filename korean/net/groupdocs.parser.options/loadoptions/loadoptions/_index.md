---
title: "LoadOptions"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "LoadOptionsgroupdocs.parser.options/loadoptions 클래스의 새 인스턴스를 초기화하고 빈 Passwordgroupdocs.parser.options/loadoptions/password, FileFormatgroupdocs.parser.options/loadoptions/fileformat을 Unknown으로 설정하며 기본 인코딩을 사용합니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 빈 [`Password`](../password), [`FileFormat`](../fileformat)을 Unknown으로 설정하며 기본 인코딩을 사용합니다.

```csharp
public LoadOptions()
```

### 참고

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 *timeout*과 함께 초기화합니다.

```csharp
public LoadOptions(TimeSpan timeout)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시간 제한 | TimeSpan | 대기할 밀리초 수를 나타내는 TimeSpan입니다. |

### 참고

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 [`FileFormat`](../fileformat)을 Unknown으로 설정하며 기본 인코딩을 사용합니다.

```csharp
public LoadOptions(string password)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |

### 참고

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 빈 [`Password`](../password)와 기본 인코딩을 사용합니다.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileFormat | FileFormat | 파일의 형식입니다. |

### 참고

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 비밀번호와 기본 인코딩을 사용합니다.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileFormat | FileFormat | 파일의 형식입니다. |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |

### 참고

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 사용자 지정 인코딩을 사용합니다.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileFormat | FileFormat | 파일의 형식입니다. |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
| encoding | Encoding | 문서의 인코딩입니다. |
| defaultAnsiEncoding | Encoding | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |

### 참고

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

[`LoadOptions`](../../loadoptions) 완전히 사용자 정의된 클래스의 새 인스턴스를 초기화합니다.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileFormat | FileFormat | 파일의 형식입니다. |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
| encoding | Encoding | 문서의 인코딩입니다. |
| defaultAnsiEncoding | Encoding | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |
| 시간 제한 | TimeSpan | 대기할 밀리초 수를 나타내는 TimeSpan입니다. |

### 참고

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 빈 [`Password`](../password)와 기본 인코딩을 사용합니다.

```csharp
public LoadOptions(FileType fileType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileType | FileType | 파일의 유형입니다. |

### 참고

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 비밀번호와 기본 인코딩을 사용합니다.

```csharp
public LoadOptions(FileType fileType, string password)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileType | FileType | 파일의 유형입니다. |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |

### 참고

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

[`LoadOptions`](../../loadoptions) 클래스의 새 인스턴스를 초기화하고 사용자 지정 인코딩을 사용합니다.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileType | FileType | 파일의 유형입니다. |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
| encoding | Encoding | 문서의 인코딩입니다. |
| defaultAnsiEncoding | Encoding | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |

### 참고

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

[`LoadOptions`](../../loadoptions) 완전히 사용자 정의된 클래스의 새 인스턴스를 초기화합니다.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileType | FileType | 파일의 유형입니다. |
| password | 문자열 | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
| encoding | Encoding | 문서의 인코딩입니다. |
| defaultAnsiEncoding | Encoding | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |
| 시간 제한 | TimeSpan | 대기할 밀리초 수를 나타내는 TimeSpan입니다. |

### 참고

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
