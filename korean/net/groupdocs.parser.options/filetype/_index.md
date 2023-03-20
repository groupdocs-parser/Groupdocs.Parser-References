---
title: FileType
second_title: .NET API 참조용 GroupDocs.Parser
description: 파일 형식을 나타냅니다. 에서 지원하는 모든 파일 형식 목록을 얻을 수 있는 방법을 제공합니다.GroupDocs.Parser .
type: docs
weight: 380
url: /ko/net/groupdocs.parser.options/filetype/
---
## FileType class

파일 형식을 나타냅니다. 에서 지원하는 모든 파일 형식 목록을 얻을 수 있는 방법을 제공합니다.**GroupDocs.Parser** .

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | 파일 이름 접미사(마침표 "." 포함) 예: ".doc". |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | 파일 유형 이름 예: "Microsoft Word 문서". |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | 파일 형식 예: "WordProcessing". |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | 파일 확장자를 파일 유형에 매핑합니다. |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 현재 여부를 결정합니다.[`FileType`](../filetype) 지정된 것과 동일합니다[`FileType`](../filetype) object. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 현재 여부를 결정합니다.[`FileType`](../filetype) 지정된 개체와 동일합니다. |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 현재 해시 코드를 반환합니다.[`FileType`](../filetype) object. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 현재 개체를 나타내는 문자열을 반환합니다. |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | 지원되는 파일 유형 검색 |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 여부를 결정합니다.[`FileType`](../filetype) 객체는 동일합니다. |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 여부를 결정합니다.[`FileType`](../filetype) 개체가 동일하지 않습니다. |

## 필드

| 이름 | 설명 |
| --- | --- |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | 확장자가 .BMP인 파일은 비트맵 디지털 이미지를 저장하는 데 사용되는 비트맵 이미지 파일을 나타냅니다. 이러한 이미지는 그래픽 어댑터와 독립적이며 DIB(장치 독립적 비트맵) 파일 형식이라고도 합니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/bmp/) . |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | Bzip2 알고리즘을 사용한 압축 파일. |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | CGM(Computer Graphics Metafile)은 벡터 그래픽(2D), 래스터 그래픽 및 텍스트를 저장하고 교환하기 위한 플랫폼 독립적인 국제 표준 메타파일 형식입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/page-description-language/cgm/) . |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM 파일 형식은 HTML 페이지 모음으로 구성된 Microsoft HTML 도움말 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/web/chm/) . |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | CSV(쉼표로 구분된 값) 확장자가 있는 파일은 쉼표로 구분된 값이 있는 데이터 레코드를 포함하는 일반 텍스트 파일 를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/spreadsheet/csv/) . |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | 확장자가 .DCM인 파일은 MRI, CT 스캔 및 초음파 이미지와 같은 환자의 의료 정보를 저장하는 디지털 이미지를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/image/dcm/) . |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB(Device Independent Bitmap) 파일은 구조가 표준 비트맵 파일(BMP)과 비슷하지만 헤더가 다른 래스터 이미지 파일입니다. 이 파일 형식 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/image/dib/) . |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | "déjà vu"로 발음되는 DjVu는 스캔한 문서 및 책, 특히 텍스트, 그림, 이미지 및 사진의 조합을 포함하는 책을 위한 그래픽 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/djvu/) . |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | 확장자가 .doc인 파일은 Microsoft Word 또는 기타 워드 프로세싱 문서에서 생성된 이진 파일 형식의 문서를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/word-processing/doc/) . |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM 파일은 매크로 실행 기능이 있는 Microsoft Word 2007 이상에서 생성된 문서입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/word-processing/docm/) . |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX는 Microsoft Word 문서의 잘 알려진 형식입니다. 2007년 Microsoft Office 2007의 release 와 함께 도입된 이 새로운 문서 형식의 구조는 일반 binary 에서 XML과 이진 파일의 조합으로 변경되었습니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/word-processing/docx/) . |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | 확장자가 .DOT인 파일은 추가 DOC 또는 DOCX 파일 생성을 위해 미리 형식이 지정된 settings 를 갖도록 Microsoft Word에서 만든 템플릿 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/word-processing/dot/) . |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | 확장자가 DOTM인 파일은 Microsoft Word 2007 이상에서 만든 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/word-processing/dotm/) . |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | DOTX 확장자를 가진 파일은 추가 DOCX 파일 생성을 위해 미리 형식이 지정된 settings 를 갖도록 Microsoft Word에서 만든 템플릿 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/word-processing/dotx/) . |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | 향상된 메타파일 형식(EMF)은 장치 독립적으로 그래픽 이미지를 저장합니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/image/emf/) . |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML 파일 형식은 Outlook 및 기타 관련 응용 프로그램을 사용하여 저장된 이메일 메시지를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/email/eml/) . |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX 파일 형식은 Apple에서 구현하고 개발합니다. Apple Mail 애플리케이션은 이메일 내보내기에 EMLX 파일 형식을 사용합니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/email/emlx/) . |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | EPS 확장자를 가진 파일은 기본적으로 단일 페이지의 모양을 설명하는 캡슐화된 PostScript 언어 프로그램 를 설명합니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/page-description-language/eps/) . |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | 확장자가 .EPUB인 파일은 발행인과 소비자를 위한 표준 디지털 출판 형식인 를 제공하는 전자책 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/ebook/epub/) . |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | FB2 확장자를 가진 파일은 eBook의 구조를 포함하는 FictionBook 2.0 eBook 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/ebook/fb2/) . |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF 또는 그래픽 교환 형식은 고도로 압축된 이미지 유형입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/gif/) . |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | 확장자가 .gz인 파일은 gzip 압축 응용 프로그램으로 만든 압축 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/compression/gz/) . |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | HTM 확장자를 가진 파일은 Google 크롬, Internet Explorer, Firefox 및 기타 여러 웹 브라우저에 표시할 웹 페이지 를 만들기 위한 Hypertext Markup Language를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/web/htm/) . |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML(Hyper Text Markup Language)은 브라우저에 표시하기 위해 만든 웹 페이지의 확장자입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/web/html/) . |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | 확장자가 ICO인 파일은 Microsoft Windows에서 애플리케이션을 나타내는 아이콘으로 사용되는 이미지 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/ico/) . |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000(J2C)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 설계 웨이블릿 기술 사용 JPEG 2000은 한 번에 모든 품질의 무손실 콘텐츠를 코딩할 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000(J2K)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 설계 웨이블릿 기술 사용 JPEG 2000은 한 번에 모든 품질의 무손실 콘텐츠를 코딩할 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000(JP2)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000(JPC)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 설계 웨이블릿 기술 사용 JPEG 2000은 한 번에 모든 품질의 무손실 콘텐츠를 코딩할 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG는 손실 압축 방법을 사용하여 저장되는 이미지 형식 유형입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/jpeg/) . |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000(JPF)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 설계 웨이블릿 기술 사용 JPEG 2000은 한 번에 모든 품질의 무손실 콘텐츠를 코딩할 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG는 손실 압축 방법을 사용하여 저장되는 이미지 형식 유형입니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/jpeg/) . |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000(JPM)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 설계 웨이블릿 기술 사용 JPEG 2000은 한 번에 모든 품질의 무손실 콘텐츠를 코딩할 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000(JPX)은 이미지 코딩 시스템이자 최신 이미지 압축 표준입니다. 설계 웨이블릿 기술 사용 JPEG 2000은 한 번에 모든 품질의 무손실 콘텐츠를 코딩할 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | Markdown 언어 방언으로 생성된 텍스트 파일은 .MD 또는 .MARKDOWN 파일 확장자로 저장됩니다. 이 파일 형식 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/word-processing/md/) . |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | MHT 확장자를 가진 파일은 다양한 응용 프로그램에서 생성할 수 있는 웹 페이지 아카이브 형식을 나타냅니다. 이 파일 형식 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/web/mhtml/) . |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | MHTML 확장자를 가진 파일은 다양한 응용 프로그램에서 생성할 수 있는 웹 페이지 아카이브 형식을 나타냅니다. 이 파일 형식 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/web/mhtml/) . |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG는 Microsoft Outlook 및 Exchange에서 전자 메일 메시지, 연락처, 약속 또는 기타 작업을 저장하는 데 사용하는 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/email/msg/) . |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | .numbers 파일 확장자를 포함하는 파일은 Apple iWork Numbers 스프레드시트 응용 프로그램에서 만든 파일입니다. |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | ODG 파일 형식은 Apache OpenOffice의 그리기 응용 프로그램에서 드로잉 요소를 벡터 이미지로 저장하는 데 사용됩니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/image/odg/) . |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | ODP 확장자를 가진 파일은 OASISOpen 표준에서 OpenOffice.org 가 사용하는 프레젠테이션 파일 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/odp/) . |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | 확장자가 ODS인 파일은 사용자가 편집할 수 있는 OpenDocument 스프레드시트 문서 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/spreadsheet/ods/) . |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT 파일은 OpenDocument 텍스트 파일 형식을 기반으로 하는 워드 프로세싱 응용 프로그램으로 만든 문서 유형입니다. 이들은 무료 OpenOffice Writer와 같은 워드 프로세서 응용 프로그램으로 생성되며 는 텍스트, 이미지, 개체 및 스타일과 같은 콘텐츠를 저장할 수 있습니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/word-processing/odt/) . |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | .ONE 확장자로 표시되는 파일은 Microsoft OneNote 응용 프로그램에서 생성됩니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/note-taking/one/) . |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST 또는 오프라인 저장소 파일은 Microsoft Outlook을 사용하여 Exchange Server에 등록 할 때 로컬 시스템의 오프라인 모드에서 사용자의 사서함 데이터를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | 확장자가 .OTP인 파일은 OASIS OpenDocument 표준 형식으로 응용 프로그램 에서 만든 프리젠테이션 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/otp/) . |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS 파일에는 OpenOffice 스프레드시트 응용 프로그램에서 사용하는 템플릿 파일이 포함되어 있습니다. |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | OTT 확장자를 가진 파일은 OASIS의 OpenDocument 표준 형식인 를 준수하는 애플리케이션에서 생성된 템플릿 문서를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/word-processing/ott/) . |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL은 HP(Hewlett Packard)에서 도입한 페이지 설명 언어 인 Printer Command Language의 약자입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/page-description-language/pcl/) . |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | PDF(Portable Document Format)는 Adobe에서 1990년대에 만든 문서 유형입니다. 이 파일 형식의 목적은 응용 프로그램 소프트웨어, 하드웨어 및 운영 체제와 독립적인 형식인 문서 및 기타 참조 자료를 표현하기 위한 표준을 도입하는 것이었습니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/view/pdf/) . |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT 파일 형식은 비트맵 이미지와 벡터 이미지 모두에 사용할 수 있는 메타 형식입니다. |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG(Portable Network Graphics)는 무손실 압축을 사용하는 래스터 이미지 파일 형식 유형을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/png/) . |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | 확장자가 .POT인 파일은 PowerPoint 97-2003 버전에서 생성된 Microsoft PowerPoint 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/pot/) . |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | 확장자가 POTM인 파일은 매크로를 지원하는 Microsoft PowerPoint 템플릿 파일입니다. POTM 파일 은 PowerPoint 2007 이상에서 생성되며 추가 프레젠테이션 파일을 생성 하는 데 사용할 수 있는 기본 설정을 포함합니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/potm/) . |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | 확장자가 .POTX인 파일은 Microsoft PowerPoint 2007 이상에서 생성된 Microsoft PowerPoint 템플릿 프레젠테이션을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/potx/) . |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS, PowerPoint 슬라이드 쇼, 파일은 슬라이드 쇼 목적으로 Microsoft PowerPoint를 사용하여 생성됩니다. PPS 파일 읽기 및 생성은 Microsoft PowerPoint 97-2003에서 지원됩니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/pps/) . |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | 확장자가 PPSM인 파일은 Microsoft PowerPoint 2007 이상에서 만든 매크로 사용 슬라이드 쇼 파일 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/ppsm/) . |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX, Power Point Slide Show, 파일은 Microsoft PowerPoint 2007 이상을 사용하여 슬라이드 쇼 목적으로 생성됩니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/ppsx/) . |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | PPT 확장자를 가진 파일은 슬라이드 쇼로 표시되는 용 슬라이드 모음으로 구성된 PowerPoint 파일을 나타냅니다. Microsoft PowerPoint 97-2003에서 사용하는 이진 파일 형식을 지정합니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/presentation/ppt/) . |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | PPTM 확장자를 가진 파일은 Microsoft PowerPoint 2007 이상 버전으로 생성된 매크로 사용 프레젠테이션 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/pptm/) . |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | PPTX 확장자를 가진 파일은 널리 사용되는 Microsoft PowerPoint 응용 프로그램으로 만든 프레젠테이션 파일입니다. 바이너리인 이전 버전의 프레젠테이션 파일 형식 PPT와 달리 PPTX 형식은 Microsoft PowerPoint open XML 프레젠테이션 파일 형식을 기반으로 됩니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/presentation/pptx/) . |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript(PS)는 데스크톱 및 전자 출판 비즈니스에서 사용되는 범용 페이지 설명 언어입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/page-description-language/ps/) . |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD, Photoshop 문서는 그래픽 디자인 및 개발에 사용되는 Adobe Photoshop의 기본 파일 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/image/psd/) . |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | 확장자가 .PST인 파일은 다양한 사용자 정보를 저장하는 Outlook 개인 저장소 파일(개인 저장소 테이블이라고도 함) 을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | 확장자가 .rar인 파일은 압축 또는 일반 형식으로 정보를 저장하기 위해 생성된 아카이브 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/compression/rar/) . |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | Microsoft에서 도입하고 문서화한 RTF(서식 있는 텍스트 형식)는 응용 프로그램 내에서 사용하기 위한 인코딩 형식의 텍스트 및 그래픽 방법을 나타냅니다. 이 형식은 다른 Microsoft 제품과 플랫폼 간 document 교환을 용이하게 하여 상호 운용성을 제공합니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/word-processing/rtf/) . |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z는 압축률이 높은 파일 및 폴더를 압축하기 위한 아카이빙 형식입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/compression/7z/) . |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | SVG 파일은 이미지 모양을 설명하기 위해 XML 기반 텍스트 format 를 사용하는 스칼라 벡터 그래픽 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/page-description-language/svg/) . |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | 확장자가 .tar인 파일은 하나 이상의 파일을 수집하기 위해 Unix 기반 유틸리티로 생성된 아카이브입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/compression/tar/) . |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | 확장자가 .TEXT인 파일은 줄 형식의 일반 텍스트를 포함하는 텍스트 문서를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/word-processing/txt/) . |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF, Tagged Image File Format은 이 파일 형식 표준을 준수하는 다양한 장치에서 사용하기 위한 래스터 이미지를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/image/tiff/) . |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF, Tagged Image File Format은 이 파일 형식 표준을 준수하는 다양한 장치에서 사용하기 위한 래스터 이미지를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/image/tiff/) . |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | 탭으로 구분된 값(TSV) 파일 형식은 일반 텍스트 형식의 탭으로 구분된 데이터를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/spreadsheet/tsv/) . |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | 확장자가 .TXT인 파일은 라인 형식의 일반 텍스트를 포함하는 텍스트 문서를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/word-processing/txt/) . |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | 알 수 없는 파일 형식을 나타냅니다. |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | Google에서 소개한 WebP는 무손실 및 손실 압축을 기반으로 하는 최신 래스터 웹 이미지 파일 형식입니다. 이미지 크기를 상당히 줄이면서 동일한 이미지 품질을 제공합니다. 이 파일 형식에 대해 자세히 알아보기[여기](https://wiki.fileformat.com/image/webp/) . |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | WMF 확장자를 가진 파일은 벡터 및 비트맵 형식 이미지 데이터를 저장하기 위한 Microsoft Windows 메타파일(WMF)을 나타냅니다. 이 파일 형식 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/image/wmf/) . |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML은 HTML 4.0의 재구성을 사용하여 XML에 마크업이 있는 텍스트 기반 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/web/xhtml/) . |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | 추가 코드를 실행하도록 설계된 보조 프로그램인 Excel 97-2003 추가 기능. VBA 프로젝트 사용을 지원합니다. |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | Excel 2010 및 Excel 2007용 XML 기반 및 매크로 사용 추가 기능 형식입니다. 추가 기능은 추가 코드를 실행하도록 설계된 보완 프로그램입니다. VBA 프로젝트 및 Excel 4.0 매크로 시트(.xlm) 사용을 지원합니다. |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | XLS 확장자를 가진 파일은 Excel 바이너리 파일 형식을 나타냅니다. 이러한 파일은 Microsoft Excel 뿐만 아니라 OpenOffice Calc 또는 Apple Numbers와 같은 기타 유사한 스프레드시트 프로그램으로 만들 수 있습니다. about 이 파일 형식 자세히 알아보기[여기](https://wiki.fileformat.com/specification/spreadsheet/xls/) . |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB 파일 형식은 Excel 통합 문서 내용을 지정하는 레코드 및 구조의 모음인 Excel 이진 파일 형식을 지정합니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/specification/spreadsheet/xlsb/) . |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | 확장자가 XLSM인 파일은 매크로를 지원하는 스프레드시트 파일 유형입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/specification/spreadsheet/xlsm/) . |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX는 Microsoft Office 2007 릴리스 와 함께 Microsoft에서 도입한 잘 알려진 Microsoft Excel 문서 형식입니다. 이 파일 format 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/specification/spreadsheet/xlsx/) . |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | 확장자가 .XLT인 파일은 Microsoft Office 제품군의 일부로 제공되는 스프레드시트 응용 프로그램인 Microsoft Excel로 만든 템플릿 파일입니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/specification/spreadsheet/xlt/) . |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM 파일 확장자는 Microsoft Excel에서 Macro-enabled 템플릿 파일로 생성된 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/specification/spreadsheet/xltm/) . |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | XLTX 확장자를 가진 파일은 Office OpenXML 파일 형식 사양을 기반으로 하는 Microsoft Excel 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/specification/spreadsheet/xltx/) . |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML은 Extensible Markup Language의 약자로 HTML 와 유사하지만 객체 정의에 태그를 사용한다는 점에서 다릅니다. 이 파일 형식 에 대해 자세히 알아보십시오.[여기](https://wiki.fileformat.com/web/xml/) . |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP 파일 확장자는 하나 이상의 파일 또는 디렉터리를 저장할 수 있는 아카이브를 나타냅니다. 이 파일 형식에 대해 자세히 알아보기 [여기](https://wiki.fileformat.com/compression/zip/) . |

### 비고

**더 알아보기:**

* [지원되는 문서 형식](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [지원되는 파일 형식 가져오기](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [문서 정보 얻기](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 또한보십시오

* 네임스페이스 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 집회 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
