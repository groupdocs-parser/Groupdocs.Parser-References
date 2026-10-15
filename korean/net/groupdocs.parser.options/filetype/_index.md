---
title: "FileType"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "파일 유형을 나타냅니다. GroupDocs.Parser에서 지원하는 모든 파일 유형 목록을 얻는 메서드를 제공합니다."
type: docs
weight: 320
url: /ko/net/groupdocs.parser.options/filetype/
---

## FileType class

파일 유형을 나타냅니다. **GroupDocs.Parser**에서 지원하는 모든 파일 유형 목록을 얻기 위한 메서드를 제공합니다.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | 파일명 접미사(마침표 "." 포함) 예: ".doc". |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | 파일 유형 이름 예: "Microsoft Word Document". |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | 파일 형식 예: "WordProcessing". |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | 파일 확장자를 파일 유형에 매핑합니다. |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 현재 [`FileType`](../filetype) 객체가 지정된 [`FileType`](../filetype) 객체와 동일한지 확인합니다. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 현재 [`FileType`](../filetype) 객체가 지정된 객체와 동일한지 확인합니다. |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 현재 [`FileType`](../filetype) 객체의 해시 코드를 반환합니다. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 현재 객체를 나타내는 문자열을 반환합니다. |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | 지원되는 파일 유형을 검색합니다 |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 두 [`FileType`](../filetype) 객체가 동일한지 확인합니다. |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 두 [`FileType`](../filetype) 객체가 동일하지 않은지 확인합니다. |

## 필드

| 이름 | 설명 |
| --- | --- |
| static readonly [AZW3](../../groupdocs.parser.options/filetype/azw3) | AZW3는 Kindle Format 8(KF8)이라고도 하며, Amazon Kindle 기기를 위해 개발된 AZW 전자책 디지털 파일 형식의 수정 버전입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/ebook/azw3/)를 클릭하십시오. |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | .BMP 확장자를 가진 파일은 비트맵 디지털 이미지를 저장하는 Bitmap Image 파일을 나타냅니다. 이러한 이미지는 그래픽 어댑터와 무관하며 디바이스 독립 비트맵(DIB) 파일 형식이라고도 합니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/image/bmp/)를 클릭하십시오. |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | Bzip2 알고리즘을 사용한 압축 파일입니다. |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile(CGM)은 벡터 그래픽(2D), 래스터 그래픽 및 텍스트를 저장하고 교환하기 위한 무료이며 플랫폼에 독립적인 국제 표준 메타파일 형식입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/page-description-language/cgm/)를 클릭하십시오. |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM 파일 형식은 HTML 페이지 모음으로 구성된 Microsoft HTML 도움말 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/web/chm/)를 클릭하십시오. |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | CSV(Comma Separated Values) 확장자를 가진 파일은 쉼표로 구분된 값으로 데이터 레코드를 포함하는 일반 텍스트 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/spreadsheet/csv/)를 클릭하십시오. |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | .DCM 확장자를 가진 파일은 MRI, CT 스캔 및 초음파 이미지와 같은 환자의 의료 정보를 저장하는 디지털 이미지를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/image/dcm/)를 클릭하십시오. |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB(Device Independent Bitmap) 파일은 표준 비트맵 파일(BMP)과 구조가 유사하지만 다른 헤더를 가진 래스터 이미지 파일입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/dib/)를 클릭하십시오. |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu는 “déjà vu”라고 발음되며, 텍스트, 그림, 이미지 및 사진이 결합된 스캔 문서와 책을 위해 설계된 그래픽 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/djvu/)를 클릭하십시오. |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | .doc 확장자를 가진 파일은 Microsoft Word 또는 기타 워드 프로세서에서 생성된 이진 파일 형식의 문서를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/doc/)를 클릭하십시오. |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM 파일은 매크로 실행 기능이 포함된 Microsoft Word 2007 이상에서 생성된 문서입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/docm/)를 클릭하십시오. |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX는 Microsoft Word 문서의 널리 알려진 형식입니다. 2007년 Microsoft Office 2007 출시와 함께 도입된 이 새로운 문서 형식은 기존의 순수 이진 구조에서 XML과 이진 파일의 조합으로 변경되었습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/docx/)를 클릭하십시오. |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | .DOT 확장자를 가진 파일은 Microsoft Word에서 만든 템플릿 파일로, 이후 DOC 또는 DOCX 파일 생성을 위한 사전 서식 설정을 포함합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/dot/)를 클릭하십시오. |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | DOTM 확장자를 가진 파일은 Microsoft Word 2007 이상에서 만든 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/dotm/)를 클릭하십시오. |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | .DOTX 확장자를 가진 파일은 Microsoft Word에서 만든 템플릿 파일로, 이후 DOCX 파일 생성을 위한 사전 서식 설정을 포함합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/dotx/)를 클릭하십시오. |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | Enhanced metafile format(EMF)은 장치에 독립적으로 그래픽 이미지를 저장합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/emf/)를 클릭하십시오. |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML 파일 형식은 Outlook 및 기타 관련 애플리케이션을 사용해 저장된 이메일 메시지를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/email/eml/)를 클릭하십시오. |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX 파일 형식은 Apple에서 구현 및 개발되었습니다. Apple Mail 애플리케이션은 이메일 내보내기에 EMLX 파일 형식을 사용합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/email/emlx/)를 클릭하십시오. |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | .EPS 확장자를 가진 파일은 단일 페이지의 모습을 설명하는 Encapsulated PostScript 언어 프로그램을 본질적으로 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/page-description-language/eps/)를 클릭하십시오. |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | .EPUB 확장자를 가진 파일은 출판사와 독자를 위한 표준 디지털 출판 형식을 제공하는 전자책 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/ebook/epub/)를 클릭하십시오. |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | .FB2 확장자를 가진 파일은 전자책의 구조를 포함하는 FictionBook 2.0 전자책 파일입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/ebook/fb2/)를 클릭하십시오. |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF(Graphic Interchange Format)는 고도로 압축된 이미지 유형입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/gif/)를 클릭하십시오. |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | .gz 확장자를 가진 파일은 gzip 압축 애플리케이션으로 만든 압축 파일입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/compression/gz/)를 클릭하십시오. |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | .HTM 확장자를 가진 파일은 Google Chrome, Internet Explorer, Firefox 등 다양한 웹 브라우저에서 표시되는 웹 페이지를 만들기 위한 Hypertext Markup Language를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/web/htm/)를 클릭하십시오. |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML(Hyper Text Markup Language)은 브라우저에서 표시되는 웹 페이지의 확장자입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/web/html/)를 클릭하십시오. |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | .ICO 확장자를 가진 파일은 Microsoft Windows에서 애플리케이션을 나타내는 아이콘으로 사용되는 이미지 파일 유형입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/ico/)를 클릭하십시오. |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000(J2C)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 웨이브릿 기술을 사용해 설계된 JPEG 2000은 어떤 품질에서도 무손실 콘텐츠를 한 번에 코딩할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하십시오. |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000(J2K)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 웨이브릿 기술을 사용해 설계된 JPEG 2000은 어떤 품질에서도 무손실 콘텐츠를 한 번에 코딩할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하십시오. |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000(JP2)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하십시오. |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000(JPC)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 웨이브릿 기술을 사용해 설계된 JPEG 2000은 어떤 품질에서도 무손실 콘텐츠를 한 번에 코딩할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하십시오. |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG은 손실 압축 방식을 사용해 저장되는 이미지 형식의 일종입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jpeg/)를 클릭하십시오. |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000(JPF)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 웨이브릿 기술을 사용해 설계된 JPEG 2000은 어떤 품질에서도 무손실 콘텐츠를 한 번에 코딩할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하십시오. |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG는 손실 압축 방식을 사용하여 저장되는 이미지 형식의 한 종류입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jpeg/)를 클릭하세요. |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 웨이브릿 기술을 사용해 설계된 JPEG 2000은 어떤 품질에서도 무손실 콘텐츠를 한 번에 코딩할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하세요. |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX)은 이미지 코딩 시스템이자 최첨단 이미지 압축 표준입니다. 웨이브릿 기술을 사용해 설계된 JPEG 2000은 어떤 품질에서도 무손실 콘텐츠를 한 번에 코딩할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/jp2/)를 클릭하세요. |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | Markdown 언어 방언으로 만든 텍스트 파일은 .MD 또는 .MARKDOWN 파일 확장자로 저장됩니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/md/)를 클릭하세요. |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | MHT 확장자를 가진 파일은 다양한 애플리케이션으로 생성할 수 있는 웹 페이지 아카이브 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/web/mhtml/)를 클릭하세요. |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | MHTML 확장자를 가진 파일은 다양한 애플리케이션으로 생성할 수 있는 웹 페이지 아카이브 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/web/mhtml/)를 클릭하세요. |
| static readonly [MOBI](../../groupdocs.parser.options/filetype/mobi) | Mobipocket 파일 형식(원래는 .prc 확장자를 사용하고 이후 .mobi로 변경)은 전자책을 위한 독점적이며 부분적으로 문서화된 바이너리 형식입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/ebook/mobi/)를 클릭하세요. |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG는 Microsoft Outlook 및 Exchange에서 이메일 메시지, 연락처, 약속 또는 기타 작업을 저장하는 데 사용하는 파일 형식입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/email/msg/)를 클릭하세요. |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | .numbers 파일 확장자를 포함하는 파일은 Apple iWork Numbers 스프레드시트 애플리케이션으로 만든 파일입니다. |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | ODG 파일 형식은 Apache OpenOffice의 Draw 애플리케이션에서 벡터 이미지로 그림 요소를 저장하는 데 사용됩니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/odg/)를 클릭하세요. |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | ODP 확장자를 가진 파일은 OASIS Open 표준에서 OpenOffice.org가 사용하는 프레젠테이션 파일 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/presentation/odp/)를 클릭하세요. |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | ODS 확장자를 가진 파일은 사용자가 편집할 수 있는 OpenDocument 스프레드시트 문서 형식을 의미합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/spreadsheet/ods/)를 클릭하세요. |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT 파일은 OpenDocument 텍스트 파일 형식을 기반으로 하는 워드 프로세싱 애플리케이션으로 만든 문서 유형입니다. 이러한 파일은 무료 OpenOffice Writer와 같은 워드 프로세서 애플리케이션으로 생성되며 텍스트, 이미지, 객체 및 스타일과 같은 내용을 포함할 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/odt/)를 클릭하세요. |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | .ONE 확장자를 가진 파일은 Microsoft OneNote 애플리케이션으로 생성됩니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/note-taking/one/)를 클릭하세요. |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST 또는 Offline Storage 파일은 Microsoft Outlook을 사용해 Exchange Server에 등록한 후 로컬 컴퓨터에서 오프라인 모드로 사용자의 메일함 데이터를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/email/ost/)를 클릭하세요. |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | .OTP 확장자를 가진 파일은 OASIS OpenDocument 표준 형식으로 애플리케이션에서 만든 프레젠테이션 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/presentation/otp/)를 클릭하세요. |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS 파일은 OpenOffice 스프레드시트 애플리케이션에서 사용하는 템플릿 파일을 포함합니다. |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | OTT 확장자를 가진 파일은 OASIS OpenDocument 표준 형식에 부합하도록 애플리케이션에서 생성된 템플릿 문서를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/word-processing/ott/)를 클릭하세요. |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL은 Hewlett Packard(HP)에서 도입한 페이지 설명 언어인 Printer Command Language의 약자입니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/page-description-language/pcl/)를 클릭하세요. |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | Portable Document Format(PDF)은 1990년대 Adobe에서 만든 문서 유형입니다. 이 파일 형식의 목적은 애플리케이션 소프트웨어, 하드웨어 및 운영 체제와 무관하게 문서와 기타 참고 자료를 표현하는 표준을 도입하는 것이었습니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/view/pdf/)를 클릭하세요. |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT 파일 형식은 비트맵 이미지와 벡터 이미지를 모두 사용할 수 있는 메타 형식입니다. |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG, Portable Network Graphics는 무손실 압축을 사용하는 래스터 이미지 파일 형식의 한 종류를 의미합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/image/png/)를 클릭하세요. |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | .POT 확장자를 가진 파일은 PowerPoint 97-2003 버전으로 만든 Microsoft PowerPoint 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/presentation/pot/). |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | POTM 확장자를 가진 파일은 매크로를 지원하는 Microsoft PowerPoint 템플릿 파일입니다. POTM 파일은 PowerPoint 2007 이상으로 생성되며 추가 프레젠테이션 파일을 만들 때 사용할 수 있는 기본 설정을 포함합니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/presentation/potm/). |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | .POTX 확장자를 가진 파일은 Microsoft PowerPoint 2007 이상으로 만든 Microsoft PowerPoint 템플릿 프레젠테이션을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [여기](https://wiki.fileformat.com/presentation/potx/). |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS, PowerPoint Slide Show, 파일은 Microsoft PowerPoint를 사용하여 슬라이드 쇼 용도로 생성됩니다. PPS 파일 읽기 및 생성은 Microsoft PowerPoint 97-2003에서 지원됩니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/presentation/pps/). |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | PPSM 확장자를 가진 파일은 Microsoft PowerPoint 2007 이상으로 만든 매크로 사용 슬라이드 쇼 파일 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/presentation/ppsm/). |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX, Power Point Slide Show, 파일은 Microsoft PowerPoint 2007 이상을 사용하여 슬라이드 쇼 용도로 생성됩니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/presentation/ppsx/). |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | PPT 확장자를 가진 파일은 슬라이드 쇼로 표시하기 위한 슬라이드 모음으로 구성된 PowerPoint 파일을 나타냅니다. 이는 Microsoft PowerPoint 97-2003에서 사용되는 바이너리 파일 형식을 지정합니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/presentation/ppt/). |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | PPTM 확장자를 가진 파일은 Microsoft PowerPoint 2007 이상 버전으로 만든 매크로 사용 프레젠테이션 파일입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/presentation/pptm/). |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | PPTX 확장자를 가진 파일은 널리 사용되는 Microsoft PowerPoint 애플리케이션으로 만든 프레젠테이션 파일입니다. 이전 바이너리 형식인 PPT와 달리 PPTX 형식은 Microsoft PowerPoint Open XML 프레젠테이션 파일 형식을 기반으로 합니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/presentation/pptx/). |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS)는 데스크톱 및 전자 출판 분야에서 사용되는 범용 페이지 설명 언어입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/page-description-language/ps/). |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD, Photoshop Document는 그래픽 디자인 및 개발에 사용되는 Adobe Photoshop의 고유 파일 형식을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/image/psd/). |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | Files with .PST extension represent Outlook Personal Storage Files (also called Personal Storage Table) that store variety of user information. Learn more about this file format [here](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | Files with .rar extension represent archive files that are created for storing information in compressed or normal form. Learn more about this file format [here](https://wiki.fileformat.com/compression/rar/). |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | Introduced and documented by Microsoft, the Rich Text Format (RTF) represents a method of encoding formatted text and graphics for use within applications. The format facilitates cross-platform document exchange with other Microsoft Products, thus serving the purpose of interoperability. Learn more about this file format [here](https://wiki.fileformat.com/word-processing/rtf/). |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z is an archiving format for compressing files and folders with a high compression ratio. Learn more about this file format [here](https://wiki.fileformat.com/compression/7z/). |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | An SVG file is a Scalar Vector Graphics file that uses XML based text format for describing the appearance of an image. Learn more about this file format [here](https://wiki.fileformat.com/page-description-language/svg/). |
| static readonly [SVGZ](../../groupdocs.parser.options/filetype/svgz) | An SVGZ file is a Scalar Vector Graphics file that uses XML based text format for describing the appearance of an image and compressed with gzip compression. |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | Files with .tar extension are archives created with Unix-based utility for collecting one or more files. Learn more about this file format [here](https://wiki.fileformat.com/compression/tar/). |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | A file with .TEXT extension represents a text document that contains plain text in the form of lines. Learn more about this file format [here](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF, Tagged Image File Format, represents raster images that are meant for usage on a variety of devices that comply with this file format standard. Learn more about this file format [here](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF, Tagged Image File Format, represents raster images that are meant for usage on a variety of devices that comply with this file format standard. Learn more about this file format [here](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | A Tab-Separated Values (TSV) file format represents data separated with tabs in plain text format. Learn more about this file format [here](https://wiki.fileformat.com/spreadsheet/tsv/). |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | A file with .TXT extension represents a text document that contains plain text in the form of lines. Learn more about this file format [here](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | Represents unknown file type. |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP, introduced by Google, is a modern raster web image file format that is based on lossless and lossy compression. It provides same image quality while considerably reducing the image size. Learn more about this file format [here](https://wiki.fileformat.com/image/webp/). |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | Files with WMF extension represent Microsoft Windows Metafile (WMF) for storing vector as well as bitmap-format images data. Learn more about this file format [here](https://wiki.fileformat.com/image/wmf/). |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | The XHTML is a text based file format with markup in the XML, using a reformulation of HTML 4.0. Learn more about this file format [here](https://wiki.fileformat.com/web/xhtml/). |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | The Excel 97-2003 Add-In, a supplemental program that is designed to run additional code. Supports the use of VBA projects. |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | Excel 2010 및 Excel 2007용 XML 기반 및 매크로 사용 가능 Add‑In 형식입니다. Add‑In은 추가 코드를 실행하도록 설계된 보조 프로그램입니다. VBA 프로젝트 및 Excel 4.0 매크로 시트(.xlm)의 사용을 지원합니다. |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | XLS 확장자를 가진 파일은 Excel 바이너리 파일 형식을 나타냅니다. 이러한 파일은 Microsoft Excel뿐만 아니라 OpenOffice Calc 또는 Apple Numbers와 같은 유사한 스프레드시트 프로그램에서도 만들 수 있습니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xls/)를 방문하십시오. |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB 파일 형식은 Excel 바이너리 파일 형식을 지정하며, 이는 Excel 워크북 내용을 정의하는 레코드와 구조의 모음입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xlsb/)를 방문하십시오. |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | XLSM 확장자를 가진 파일은 매크로를 지원하는 스프레드시트 파일 유형입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xlsm/)를 방문하십시오. |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX는 Microsoft Office 2007 출시와 함께 Microsoft에서 도입한 Microsoft Excel 문서의 잘 알려진 형식입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xlsx/)를 방문하십시오. |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | .XLT 확장자를 가진 파일은 Microsoft Office 제품군의 일부인 스프레드시트 애플리케이션 Microsoft Excel로 만든 템플릿 파일입니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xlt/)를 방문하십시오. |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM 파일 확장자는 Microsoft Excel에서 매크로 사용 가능 템플릿 파일로 생성된 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xltm/)를 방문하십시오. |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | XLTX 확장자를 가진 파일은 Office OpenXML 파일 형식 사양을 기반으로 하는 Microsoft Excel 템플릿 파일을 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/specification/spreadsheet/xltx/)를 방문하십시오. |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML은 Extensible Markup Language의 약자로, HTML과 유사하지만 객체를 정의하기 위해 태그를 사용하는 점에서 다릅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/web/xml/)를 방문하십시오. |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP 파일 확장자는 하나 이상의 파일이나 디렉터리를 보관할 수 있는 아카이브를 나타냅니다. 이 파일 형식에 대해 자세히 알아보려면 [here](https://wiki.fileformat.com/compression/zip/)를 방문하십시오. |

### 비고

**Learn more:**

* [Supported Document Formats](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [Get supported file formats](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 참고

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
