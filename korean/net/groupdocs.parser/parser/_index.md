---
title: Parser
second_title: .NET API 참조용 GroupDocs.Parser
description: 텍스트 이미지 컨테이너 추출 및 구문 분석 기능을 제어하는 기본 클래스를 나타냅니다.
type: docs
weight: 640
url: /ko/net/groupdocs.parser/parser/
---
## Parser class

텍스트, 이미지, 컨테이너 추출 및 구문 분석 기능을 제어하는 기본 클래스를 나타냅니다.

```csharp
public sealed class Parser : IDisposable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 데이터베이스에서 데이터를 추출하는 클래스. |
| [Parser](parser#constructor)(EmailConnection) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 원격 이메일 서버에서 데이터를 추출하는 클래스. |
| [Parser](parser#constructor_4)(Stream) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 클래스. |
| [Parser](parser#constructor_8)(string) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 클래스. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 데이터베이스에서 데이터를 추출하는 클래스. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 원격 이메일 서버에서 데이터를 추출하는 클래스. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 와 수업[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 와 수업[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 와 수업[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 와 수업[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 와 수업[`LoadOptions`](../../groupdocs.parser.options/loadoptions) 및[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | 의 새 인스턴스를 초기화합니다.[`Parser`](../parser) 와 수업[`LoadOptions`](../../groupdocs.parser.options/loadoptions) 및[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | 지원되는 기능을 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | 페이지 미리보기 가져오기. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | 문서에서 바코드를 추출합니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | 문서 페이지에서 바코드를 추출합니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | 사용자 지정 옵션 (바코드가 포함된 직사각형 영역 설정)를 사용하여 문서에서 바코드를 추출합니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | 사용자 지정 옵션 (바코드가 포함된 직사각형 영역 설정)를 사용하여 문서 페이지에서 바코드를 추출합니다. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | 첨부 파일, ZIP 아카이브 등을 포함하는 형식으로 작업하기 위해 문서에서 컨테이너 개체를 추출합니다. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | 문서에 대한 일반 정보를 반환합니다. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | 문서에서 서식 있는 텍스트를 추출합니다. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | 문서 페이지에서 서식 있는 텍스트를 추출합니다. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | 문서에서 하이라이트를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | 문서에서 하이퍼링크를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | 문서 페이지에서 하이퍼링크를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | 사용자 지정 옵션 (하이퍼링크가 포함된 사각형 영역 설정)를 사용하여 문서에서 하이퍼링크를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | 사용자 지정 옵션 (하이퍼링크가 포함된 사각형 영역 설정)를 사용하여 문서 페이지에서 하이퍼링크를 추출합니다. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | 문서에서 이미지를 추출합니다. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | 문서 페이지에서 이미지를 추출합니다. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | 사용자 지정 옵션 (이미지가 포함된 직사각형 영역 설정)를 사용하여 문서에서 이미지를 추출합니다. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | 사용자 지정 옵션 (이미지가 포함된 직사각형 영역 설정)를 사용하여 문서 페이지에서 이미지를 추출합니다. |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | 문서에서 메타데이터를 추출합니다. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | 문서에서 구조화된 텍스트를 추출합니다. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | 문서에서 테이블을 추출합니다. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | 문서 페이지에서 표를 추출합니다. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | 문서에서 텍스트를 추출합니다. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | 문서 페이지에서 텍스트를 추출합니다. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | 텍스트 옵션을 사용하여 문서에서 텍스트 페이지를 추출합니다(원시 빠른 텍스트 추출 모드 활성화). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | 텍스트 옵션을 사용하여 문서 페이지에서 텍스트를 추출합니다(원시 빠른 텍스트 추출 모드 활성화). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | 문서에서 텍스트 영역을 추출합니다. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | 문서 페이지에서 텍스트 영역을 추출합니다. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | 사용자 지정 옵션(정규식, 대/소문자 구분 등)을 사용하여 문서에서 텍스트 영역을 추출합니다. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | 사용자 지정 옵션(정규식, 대/소문자 구분 등)을 사용하여 문서 페이지에서 텍스트 영역을 추출합니다. |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | 문서에서 목차를 추출합니다. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | 사용자가 생성한 템플릿으로 문서를 구문 분석합니다. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | 문서 양식을 구문 분석합니다. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | 검색*keyword* 문서에서. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | 검색*keyword*검색 옵션(정규식, 대/소문자 구분 등)을 사용하여 문서에서. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | 파일에 대한 일반 정보를 반환합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | 파일에 대한 일반 정보를 반환합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | 파일에 대한 일반 정보를 반환합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | 파일에 대한 일반 정보를 반환합니다. |

### 또한보십시오

* 네임스페이스 [GroupDocs.Parser](../../groupdocs.parser)
* 집회 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
