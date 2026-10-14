---
title: "com.groupdocs.parser.options"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "이 패키지는 문서에서 데이터를 구문 분석할 때 추가 옵션을 지정할 수 있는 클래스를 제공합니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.parser.options/
---

이 패키지는 문서에서 데이터를 구문 분석할 때 추가 옵션을 지정할 수 있는 클래스를 제공합니다.



## 클래스

| 클래스 | 설명 |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | 바코드 추출에 사용되는 옵션을 제공합니다. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | 문서 정보를 나타냅니다. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | 이메일 연결 정보를 나타냅니다. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | EWS 프로토콜에 대한 이메일 연결 정보를 나타냅니다. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | IMAP 프로토콜에 대한 이메일 연결 정보를 나타냅니다. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | POP 프로토콜에 대한 이메일 연결 정보를 나타냅니다. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | 외부 리소스 로드를 위한 핸들러를 제공합니다. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | 다음 메서드인 [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-)에 대한 데이터를 제공합니다. |
| [Features](../com.groupdocs.parser.options/features) | 지원되는 기능 목록을 나타냅니다. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | 파일 정보를 나타냅니다. |
| [FileType](../com.groupdocs.parser.options/filetype) | 파일 유형을 나타냅니다. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | 서식이 지정된 텍스트 추출에 사용되는 옵션을 제공합니다. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | 검색 시나리오에서 찾은 텍스트 주변의 텍스트 블록(하이라이트)을 추출하는 데 사용되는 옵션을 제공합니다. |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | 이미지 추출에 사용되는 옵션을 제공합니다. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | 파일을 열 때 사용되는 옵션을 제공합니다. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | OCR 기능을 제공합니다. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | OCR 이벤트에 대한 핸들러를 제공합니다. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | OCR 커넥터에 사용되는 옵션을 제공합니다. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | 페이지 영역 추출에 사용되는 옵션을 제공합니다. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | 문서 페이지 정보를 나타냅니다. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | 페이지가 렌더링되는 방식에 대한 정보를 나타냅니다. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | 페이지 표 영역 추출에 사용되는 옵션을 제공합니다. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | 페이지 텍스트 영역 추출에 사용되는 옵션을 제공합니다. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 사용자 정의하는 데 사용되는 설정을 제공합니다. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | 미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | 텍스트 검색에 사용되는 옵션을 제공합니다. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | 텍스트 문서 정보를 나타냅니다. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | 텍스트 추출에 사용되는 옵션을 제공합니다. |

## 인터페이스

| 인터페이스 | 설명 |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | 페이지 미리보기 데이터를 쓰기 위해 스트림을 반환하는 대리자를 나타냅니다. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | 문서 정보를 나타냅니다. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | 데이터 추출 중 이벤트와 오류를 기록하는 데 사용되는 로거의 인터페이스를 정의합니다. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | 문서 페이지가 렌더링되기 전에 호출되는 메서드를 나타냅니다. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | 스트림을 해제하는 메서드를 나타냅니다. 이 스트림은 [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) 대리자에 의해 생성됩니다. |

## 열거형

| 열거형 | 설명 |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | 파일 유형을 정의합니다. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | 파일 유형 감지 모드를 정의합니다. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | 서식 있는 텍스트 모드를 정의합니다. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | 이미지 형식을 정의합니다. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | 지원되는 미리보기 형식을 나타냅니다. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | 품질 수준을 정의합니다. |
