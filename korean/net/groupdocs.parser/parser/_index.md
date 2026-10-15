---
title: "파서"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "텍스트 이미지 컨테이너 추출 및 파싱 기능을 제어하는 주요 클래스를 나타냅니다."
type: docs
weight: 30
url: /ko/net/groupdocs.parser/parser/
---

## Parser class

텍스트, 이미지, 컨테이너 추출 및 구문 분석 기능을 제어하는 주요 클래스를 나타냅니다.

```csharp
public sealed class Parser : IDisposable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 데이터베이스에서 데이터를 추출합니다. |
| [Parser](parser#constructor)(EmailConnection) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 원격 이메일 서버에서 데이터를 추출합니다. |
| [Parser](parser#constructor_4)(Stream) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스의. |
| [Parser](parser#constructor_8)(string) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스의. |
| [Parser](parser#constructor_12)(Uri) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 URI에서 데이터를 추출합니다. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 데이터베이스에서 데이터를 추출합니다. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 원격 이메일 서버에서 데이터를 추출합니다. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 [`LoadOptions`](../../groupdocs.parser.options/loadoptions)와 함께. |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 [`ParserSettings`](../../groupdocs.parser.options/parsersettings)와 함께. |
| [Parser](parser#constructor_9)(string, LoadOptions) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 [`LoadOptions`](../../groupdocs.parser.options/loadoptions)와 함께. |
| [Parser](parser#constructor_11)(string, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 [`ParserSettings`](../../groupdocs.parser.options/parsersettings)와 함께. |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 *loadOptions*와 함께 URI에서 데이터를 추출합니다. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 *parserSettings*와 함께 URI에서 데이터를 추출합니다. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 [`LoadOptions`](../../groupdocs.parser.options/loadoptions)와 [`ParserSettings`](../../groupdocs.parser.options/parsersettings)와 함께. |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 [`LoadOptions`](../../groupdocs.parser.options/loadoptions)와 [`ParserSettings`](../../groupdocs.parser.options/parsersettings)와 함께. |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | 새 인스턴스를 초기화합니다 [`Parser`](../parser) 클래스를 사용하여 *loadOptions*와 *parserSettings*와 함께 URI에서 데이터를 추출합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | 지원되는 기능을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | 관리되지 않는 리소스를 해제, 릴리스 또는 재설정과 관련된 애플리케이션 정의 작업을 수행합니다. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | 템플릿 위치와 크기의 자동 조정을 위한 필드를 생성합니다. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | 페이지 미리보기를 가져옵니다. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | 문서에서 주석을 추출합니다. 현재는 PDF 형식만 지원됩니다. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | 문서 페이지에서 주석을 추출합니다. 현재는 PDF 형식만 지원됩니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | 문서에서 바코드를 추출합니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | 맞춤 옵션을 사용하여 문서에서 바코드를 추출합니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | 문서 페이지에서 바코드를 추출합니다. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | 맞춤 옵션을 사용하여 문서 페이지에서 바코드를 추출합니다. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | 첨부 파일, ZIP 아카이브 등을 포함하는 형식과 작업하기 위해 문서에서 컨테이너 객체를 추출합니다. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | 문서에 대한 일반 정보를 반환합니다. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | 문서에서 서식이 지정된 텍스트를 추출합니다. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | 문서 페이지에서 서식이 지정된 텍스트를 추출합니다. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | 문서에서 하이라이트를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | 문서에서 하이퍼링크를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | 문서 페이지에서 하이퍼링크를 추출합니다. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | 맞춤 옵션을 사용하여 문서에서 하이퍼링크를 추출합니다 (하이퍼링크가 포함된 사각형 영역을 설정하기 위해). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | 맞춤 옵션을 사용하여 문서 페이지에서 하이퍼링크를 추출합니다 (하이퍼링크가 포함된 사각형 영역을 설정하기 위해). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | 문서에서 이미지를 추출합니다. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | 문서 페이지에서 이미지를 추출합니다. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | 맞춤 옵션을 사용하여 문서에서 이미지를 추출합니다 (이미지가 포함된 사각형 영역을 설정하기 위해). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | 맞춤 옵션을 사용하여 문서 페이지에서 이미지를 추출합니다 (이미지가 포함된 사각형 영역을 설정하기 위해). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | 문서에서 메타데이터를 추출합니다. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | 문서 페이지 미리보기를 생성합니다. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | 맞춤 옵션을 사용하여 문서 페이지 미리보기를 생성합니다. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | 문서에서 구조화된 텍스트를 추출합니다. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | 문서에서 표를 추출합니다. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | 문서 페이지에서 표를 추출합니다. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | 문서에서 표를 추출합니다. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | 문서 페이지에서 표를 추출합니다. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | 문서에서 텍스트를 추출합니다. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | 문서 페이지에서 텍스트를 추출합니다. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | 텍스트 옵션을 사용하여 문서에서 텍스트 페이지를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | 텍스트 옵션을 사용하여 문서 페이지에서 텍스트를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | 문서에서 텍스트 영역을 추출합니다. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | 문서 페이지에서 텍스트 영역을 추출합니다. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | 맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 텍스트 영역을 추출합니다. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | 맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서 페이지에서 텍스트 영역을 추출합니다. |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | 문서에서 목차를 추출합니다. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | 워크시트 셀을 추출합니다. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | 맞춤 옵션을 사용하여 워크시트 셀을 추출합니다. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | 스프레드시트의 모든 워크시트에 대한 정보를 추출합니다. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | 워크시트에 대한 정보를 추출합니다. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | 사용자 생성 템플릿으로 문서를 구문 분석합니다. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | 맞춤 옵션을 사용하여 사용자 생성 템플릿으로 문서를 구문 분석합니다. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | 제공된 컬렉션에서 가장 적합한 템플릿을 선택한 다음, 선택된 템플릿을 사용해 문서를 구문 분석합니다. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | 문서 양식을 구문 분석합니다. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | 문서에서 *keyword*를 검색합니다. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | 검색 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 *keyword*를 검색합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | 파일에 대한 일반 정보를 반환합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | 파일에 대한 일반 정보를 반환합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | 파일에 대한 일반 정보를 반환합니다. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | 파일에 대한 일반 정보를 반환합니다. |

### 참고

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
