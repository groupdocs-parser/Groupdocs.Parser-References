---
title: "FileType"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar filtypen."
type: docs
weight: 20
url: /sv/java/com.groupdocs.parser.options/filetype/
---
**Inheritance:**
java.lang.Object
```
public class FileType
```

Representerar filtypen. Tillhandahåller metoder för att hämta en lista över alla filtyper som stöds av GroupDocs.Parser.

**Learn more:**

* [Supported File Formats](../https://docs.groupdocs.com/display/parserjava/Supported+Document+Formats)
* [Get supported file formats](../https://docs.groupdocs.com/display/parserjava/Get+supported+file+formats)
* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Unknown](#Unknown) | Representerar okänd filtyp. |
|
|  | [DOC](#DOC) | Filer med .doc-tillägg representerar dokument som genererats av Microsoft Word eller andra ordbehandlingsdokument i binärt filformat. |
|
|  | [DOT](#DOT) | Filer med .DOT-tillägg är mallfiler skapade av Microsoft Word för att ha förformaterade inställningar för generering av ytterligare DOC- eller DOCX-filer. |
|
|  | [DOCX](#DOCX) | DOCX är ett välkänt format för Microsoft Word-dokument. |
|
|  | [DOCM](#DOCM) | DOCM-filer är dokument som genererats av Microsoft Word 2007 eller senare med möjlighet att köra makron. |
|
|  | [DOTX](#DOTX) | Filer med .DOTX-tillägg är mallfiler skapade av Microsoft Word för att ha förformaterade inställningar för generering av ytterligare DOCX-filer. |
|
|  | [DOTM](#DOTM) | En fil med .DOTM-tillägg representerar en mallfil skapad med Microsoft Word 2007 eller senare. |
|
|  | [TXT](#TXT) | En fil med .TXT-tillägg representerar ett textdokument som innehåller ren text i form av rader. |
|
|  | [TEXT](#TEXT) | En fil med .TEXT-tillägg representerar ett textdokument som innehåller ren text i form av rader. |
|
|  | [ODT](#ODT) | ODT-filer är en typ av dokument som skapats med ordbehandlingsprogram baserade på OpenDocument Text-filformat. |
|
|  | [OTT](#OTT) | Filer med .OTT-tillägg representerar mall-dokument som genererats av program i enlighet med OASIS OpenDocument-standardformatet. |
|
|  | [RTF](#RTF) | Introducerat och dokumenterat av Microsoft, Rich Text Format (RTF) representerar en metod för att koda formaterad text och grafik för användning i program. |
|
|  | [PDF](#PDF) | Portable Document Format (PDF) är en typ av dokument som skapades av Adobe på 1990-talen. |
|
|  | [HTM](#HTM) | Filer med .HTM-tillägg representerar Hypertext Markup Language för att skapa webbsidor för visning i webbläsare såsom Google Chrome, Internet Explorer, Firefox och ett antal andra. |
|
|  | [HTML](#HTML) | HTML (Hyper Text Markup Language) är filändelsen för webbsidor skapade för visning i webbläsare. |
|
|  | [XHTML](#XHTML) | XHTML är ett textbaserat filformat med markup i XML, med en omformulering av HTML 4.0. |
|
|  | [MHT](#MHT) | Filer med .MHT-tillägg representerar ett webbsidesarkivformat som kan skapas av ett antal olika program. |
|
|  | [MHTML](#MHTML) | Filer med .MHTML-tillägg representerar ett webbsidesarkivformat som kan skapas av ett antal olika program. |
|
|  | [XML](#XML) | XML står för Extensible Markup Language som liknar HTML men skiljer sig åt genom att använda taggar för att definiera objekt. |
|
|  | [MD](#MD) | Textfiler skapade med Markdown-språkdialekter sparas med filändelsen .MD eller .MARKDOWN. |
|
|  | [FB2](#FB2) | Filer med .FB2-tillägg är FictionBook 2.0-e-bokfiler som innehåller e-bokens struktur. |
|
|  | [CHM](#CHM) | CHM-filformatet representerar Microsoft HTML-hjälpfil som består av en samling HTML-sidor. |
|
|  | [EPUB](#EPUB) | Filer med .EPUB‑extension är ett e‑bokfilformat som tillhandahåller ett standardiserat digitalt publiceringsformat för utgivare och konsumenter. |
|
|  | [AZW3](#AZW3) | AZW3, även känt som Kindle Format 8 (KF8), är den modifierade versionen av det digitala AZW‑ebookfilformatet som utvecklats för Amazon Kindle‑enheter. |
|
|  | [MOBI](#MOBI) | Mobipocket‑filformatet (ursprungligen med filändelsen .prc och senare .mobi) är ett proprietärt, delvis dokumenterat binärt format för e‑böcker. |
|
|  | [XLS](#XLS) | Filer med XLS‑extension representerar Excel Binary File Format. |
|
|  | [XLSX](#XLSX) | XLSX är ett välkänt format för Microsoft Excel‑dokument som introducerades av Microsoft med lanseringen av Microsoft Office 2007. |
|
|  | [XLSM](#XLSM) | Filer med XLSM‑extension är en typ av kalkylbladsfiler som stödjer makron. |
|
|  | [XLSB](#XLSB) | XLSB‑filformatet specificerar Excel Binary File Format, vilket är en samling poster och strukturer som definierar innehållet i en Excel‑arbetsbok. |
|
|  | [XLT](#XLT) | Filer med .XLT‑extension är mallfiler skapade med Microsoft Excel, som är ett kalkylprogram som ingår i Microsoft Office‑sviten. |
|
|  | [XLTX](#XLTX) | Filer med XLTX‑extension representerar Microsoft Excel‑mallfiler som är baserade på specifikationerna för Office OpenXML‑filformatet. |
|
|  | [XLTM](#XLTM) | XLTM‑filändelsen representerar filer som genereras av Microsoft Excel som makroaktiverade mallfiler. |
|
|  | [XLA](#XLA) | Excel 97-2003‑tillägget, ett kompletterande program som är avsett att köra ytterligare kod. |
|
|  | [XLAM](#XLAM) | Det XML‑baserade och makroaktiverade tilläggsformatet för Excel 2010 och Excel 2007. |
|
|  | [CSV](#CSV) | Filer med CSV‑ (Comma Separated Values)‑extension representerar textfiler som innehåller dataposter med kommaseparerade värden. |
|
|  | [TSV](#TSV) | Ett Tab‑Separated Values (TSV)‑filformat representerar data separerade med tabbar i ett vanligt textformat. |
|
|  | [ODS](#ODS) | Filer med ODS‑extension står för OpenDocument Spreadsheet‑dokumentformat som kan redigeras av användaren. |
|
|  | [OTS](#OTS) | OTS‑filerna innehåller mallfiler som används av OpenOffice‑kalkylprogrammet. |
|
|  | [NUMBERS](#NUMBERS) | Filer med .numbers‑filändelse är filer som skapats av Apple iWork Numbers‑kalkylprogrammet. |
|
|  | [PPT](#PPT) | En fil med PPT‑extension representerar en PowerPoint‑fil som består av en samling bilder för visning som bildspel. |
|
|  | [PPTX](#PPTX) | Filer med PPTX‑extension är presentationsfiler skapade med det populära Microsoft PowerPoint‑programmet. |
|
|  | [PPS](#PPS) | PPS, PowerPoint Slide Show, filer skapas med Microsoft PowerPoint för bildspelsändamål. |
|
|  | [PPSX](#PPSX) | PPSX, Power Point Slide Show, filer skapas med Microsoft PowerPoint 2007 och senare för bildspelsändamål. |
|
|  | [ODP](#ODP) | Filer med ODP‑extension representerar presentationsfilformatet som används av OpenOffice.org i OASISOpen‑standarden. |
|
|  | [POT](#POT) | Filer med .POT‑extension representerar Microsoft PowerPoint‑mallfiler skapade av PowerPoint‑versionerna 97‑2003. |
|
|  | [PPTM](#PPTM) | Filer med PPTM‑extension är makroaktiverade presentationsfiler som skapats med Microsoft PowerPoint 2007 eller senare versioner. |
|
|  | [POTX](#POTX) | Filer med .POTX‑extension representerar Microsoft PowerPoint‑mallpresentationer som skapats med Microsoft PowerPoint 2007 och senare. |
|
|  | [POTM](#POTM) | Filer med POTM‑tillägg är Microsoft PowerPoint‑mallfiler med stöd för makron. |
|
|  | [PPSM](#PPSM) | Filer med PPSM‑tillägg representerar makroaktiverat bildspelsfilformat skapat med Microsoft PowerPoint 2007 eller senare. |
|
|  | [OTP](#OTP) | Filer med .OTP‑tillägg representerar presentationsmallfiler som skapats av program i OASIS OpenDocument‑standardformat. |
|
|  | [MSG](#MSG) | MSG är ett filformat som används av Microsoft Outlook och Exchange för att lagra e‑postmeddelanden, kontakter, möten eller andra uppgifter. |
|
|  | [EML](#EML) | EML‑filformatet representerar e‑postmeddelanden som sparats med Outlook och andra relevanta program. |
|
|  | [EMLX](#EMLX) | EMLX‑filformatet implementeras och utvecklas av Apple. |
|
|  | [PST](#PST) | Filer med .PST‑tillägg representerar Outlook Personal Storage Files (även kallade Personal Storage Table) som lagrar en mängd användarinformation. |
|
|  | [OST](#OST) | OST‑ eller Offline Storage‑filer representerar användarens brevlådedata i offlineläge på den lokala maskinen efter registrering mot Exchange Server med Microsoft Outlook. |
|
|  | [ONE](#ONE) | Filer med .ONE‑tillägg skapas av Microsoft OneNote‑programmet. |
|
|  | [ZIP](#ZIP) | ZIP‑tillägget representerar arkiv som kan innehålla en eller flera filer eller kataloger. |
|
|  | [SEVENZ](#SEVENZ) | 7z är ett arkiveringsformat för att komprimera filer och mappar med hög komprimeringsgrad. |
|
|  | [RAR](#RAR) | Filer med .rar‑tillägg representerar arkivfiler som skapas för att lagra information i komprimerad eller normal form. |
|
|  | [TAR](#TAR) | Filer med .tar‑tillägg är arkiv skapade med ett Unix‑baserat verktyg för att samla en eller flera filer. |
|
|  | [GZ](#GZ) | Filer med .gz‑tillägg är komprimerade filer skapade med gzip‑komprimeringsprogram. |
|
|  | [BZ2](#BZ2) | Komprimerad fil med Bzip2‑algoritmen. |
|
|  | [TIF](#TIF) | TIF, Tagged Image File Format, representerar rasterbilder som är avsedda för användning på en mängd enheter som följer detta filformatstandard. |
|
|  | [TIFF](#TIFF) | TIFF, Tagged Image File Format, representerar rasterbilder som är avsedda för användning på en mängd enheter som följer detta filformatstandard. |
|
|  | [JPG](#JPG) | En JPG är en typ av bildformat som sparas med en förlustkomprimeringsmetod. |
|
|  | [JPEG](#JPEG) | En JPEG är en typ av bildformat som sparas med en förlustkomprimeringsmetod. |
|
|  | [PNG](#PNG) | PNG, Portable Network Graphics, avser en typ av rasterbildfilformat som använder förlustfri kompression. |
|
|  | [GIF](#GIF) | En GIF eller Graphical Interchange Format är en typ av starkt komprimerad bild. |
|
|  | [BMP](#BMP) | Filer med .BMP‑tillägg representerar Bitmap Image‑filer som används för att lagra bitmap‑digitala bilder. |
|
|  | [ICO](#ICO) | Filer med ICO‑tillägg är bildfiltyper som används som ikon för att representera ett program på Microsoft Windows. |
|
|  | [JP2](#JP2) | JPEG 2000 (JP2) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. |
|
|  | [JPF](#JPF) | JPEG 2000 (JPF) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. |
|
|  | [JPX](#JPX) | JPEG 2000 (JPX) är ett bildkodningssystem och en banbrytande bildkomprimeringsstandard. |
|
|  | [JPM](#JPM) | JPEG 2000 (JPM) är ett bildkodningssystem och en banbrytande bildkomprimeringsstandard. |
|
|  | [J2C](#J2C) | JPEG 2000 (J2C) är ett bildkodningssystem och en banbrytande bildkomprimeringsstandard. |
|
|  | [J2K](#J2K) | JPEG 2000 (J2K) är ett bildkodningssystem och en banbrytande bildkomprimeringsstandard. |
|
|  | [JPC](#JPC) | JPEG 2000 (JPC) är ett bildkodningssystem och en banbrytande bildkomprimeringsstandard. |
|
|  | [DIB](#DIB) | En DIB (Device Independent Bitmap) fil är en rasterbildfil som är lik strukturen som standard Bitmap-filer (BMP) men har ett annat huvud. |
|
|  | [WMF](#WMF) | Filer med WMF‑tillägg representerar Microsoft Windows Metafile (WMF) för lagring av både vektor‑ och bitmap‑format bilddata. |
|
|  | [EMF](#EMF) | Enhanced metafile format (EMF) lagrar grafiska bilder enhetsoberoende. |
|
|  | [WEBP](#WEBP) | WebP, introducerat av Google, är ett modernt rasterwebb‑bildfilformat som bygger på förlustfri och förlustkomprimering. |
|
|  | [DJVU](#DJVU) | DjVu är ett grafikfilformat avsett för skannade dokument och böcker, särskilt de som innehåller en kombination av text, teckningar, bilder och fotografier. |
|
|  | [CGM](#CGM) | Computer Graphics Metafile (CGM) är ett fritt, plattformsoberoende, internationellt standardmetafilformat för lagring och utbyte av vektorgrafik (2D), rastergrafik och text. |
|
|  | [PCL](#PCL) | PCL står för Printer Command Language, vilket är ett sidbeskrivningsspråk introducerat av Hewlett Packard (HP). |
|
|  | [PSD](#PSD) | PSD, Photoshop Document, representerar Adobe Photoshops inhemska filformat som används för grafisk design och utveckling. |
|
|  | [DCM](#DCM) | Filer med .DCM‑tillägg representerar digitala bilder som lagrar medicinsk information om patienter såsom MR‑bilder, CT‑skanningar och ultraljudsbilder. |
|
|  | [PS](#PS) | PostScript (PS) är ett allmänt syftande sidbeskrivningsspråk som används inom skrivbordspublicering och elektronisk publicering. |
|
|  | [EPS](#EPS) | Filer med EPS‑tillägg beskriver i huvudsak ett Encapsulated PostScript‑språkprogram som beskriver utseendet på en enskild sida. |
|
|  | [ODG](#ODG) | ODG‑filformatet används av Apache OpenOffice:s Draw‑applikation för att lagra ritningselement som en vektorbild. |
|
|  | [SVG](#SVG) | En SVG‑fil är en Scalar Vector Graphics‑fil som använder ett XML‑baserat textformat för att beskriva en bilds utseende. |
|
|  | [PICT](#PICT) | PICT‑filformatet är ett meta‑format som kan användas för både bitmap‑bilder och vektor‑bilder. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Filtypnamn t.ex. |
|
|  | [getExtension()](#getExtension--) | Filnamnstillägg (inklusive punkt ".") t.ex. |
|
|  | [getFormat()](#getFormat--) | Filformat t.ex. |
|
| [equals(Object object)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
| [toString()](#toString--) |  |
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Kopplar filändelse till filtyp. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Hämtar stödjade filtyper. |
|
### Unknown {#Unknown}
```
public static final FileType Unknown
```


Representerar okänd filtyp.


### DOC {#DOC}
```
public static final FileType DOC
```


Filer med .doc‑tillägg representerar dokument som genererats av Microsoft Word eller andra ordbehandlingsdokument i binärt filformat. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/doc/).


### DOT {#DOT}
```
public static final FileType DOT
```


Filer med .DOT‑tillägg är mallfiler som skapats av Microsoft Word för att ha förformaterade inställningar för generering av ytterligare DOC‑ eller DOCX‑filer. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/dot/).


### DOCX {#DOCX}
```
public static final FileType DOCX
```


DOCX är ett välkänt format för Microsoft Word‑dokument. Introducerat från 2007 med lanseringen av Microsoft Office 2007 ändrades strukturen för detta nya dokumentformat från ren binär till en kombination av XML‑ och binära filer. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/docx/).


### DOCM {#DOCM}
```
public static final FileType DOCM
```


DOCM‑filer är dokument som genererats av Microsoft Word 2007 eller senare med möjlighet att köra makron. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/docm/).


### DOTX {#DOTX}
```
public static final FileType DOTX
```


Filer med DOTX‑tillägg är mallfiler som skapats av Microsoft Word för att ha förformaterade inställningar för generering av ytterligare DOCX‑filer. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/dotx/).


### DOTM {#DOTM}
```
public static final FileType DOTM
```


En fil med DOTM‑tillägg representerar en mallfil skapad med Microsoft Word 2007 eller senare. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/dotm/).


### TXT {#TXT}
```
public static final FileType TXT
```


En fil med .TXT‑tillägg representerar ett textdokument som innehåller vanlig text i form av rader. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/txt/).


### TEXT {#TEXT}
```
public static final FileType TEXT
```


En fil med .TEXT‑tillägg representerar ett textdokument som innehåller vanlig text i form av rader. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/txt/).


### ODT {#ODT}
```
public static final FileType ODT
```


ODT‑filer är en typ av dokument som skapats med ordbehandlingsprogram baserade på OpenDocument Text‑filformatet. Dessa skapas med ordbehandlingsprogram som det kostnadsfria OpenOffice Writer och kan innehålla innehåll såsom text, bilder, objekt och stilar. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/odt/).


### OTT {#OTT}
```
public static final FileType OTT
```


Filer med OTT‑tillägg representerar mall‑dokument som genereras av program i enlighet med OASIS OpenDocument‑standardformatet. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/ott/).


### RTF {#RTF}
```
public static final FileType RTF
```


Introducerat och dokumenterat av Microsoft, Rich Text Format (RTF) är en metod för att koda formaterad text och grafik för användning i program. Formatet underlättar plattformsoberoende dokumentutbyte med andra Microsoft‑produkter, vilket tjänar interoperabilitetens syfte. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/rtf/).


### PDF {#PDF}
```
public static final FileType PDF
```


Portable Document Format (PDF) är en typ av dokument som skapades av Adobe på 1990‑talen. Syftet med detta filformat var att införa en standard för representation av dokument och annat referensmaterial i ett format som är oberoende av programvara, hårdvara samt operativsystem. Läs mer om detta filformat [här](../https://wiki.fileformat.com/view/pdf/).


### HTM {#HTM}
```
public static final FileType HTM
```


Filer med HTM‑tillägg representerar Hypertext Markup Language för att skapa webbsidor för visning i webbläsare såsom Google Chrome, Internet Explorer, Firefox och ett antal andra. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/htm/).


### HTML {#HTML}
```
public static final FileType HTML
```


HTML (Hyper Text Markup Language) är filändelsen för webbsidor som skapats för visning i webbläsare. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/html/).


### XHTML {#XHTML}
```
public static final FileType XHTML
```


XHTML är ett textbaserat filformat med markup i XML, som använder en omformulering av HTML 4.0. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/xhtml/).


### MHT {#MHT}
```
public static final FileType MHT
```


Filer med MHT‑tillägg representerar ett webbsidesarkivformat som kan skapas av ett antal olika program. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/mhtml/).


### MHTML {#MHTML}
```
public static final FileType MHTML
```


Filer med MHTML‑tillägg representerar ett webbsidesarkivformat som kan skapas av ett antal olika program. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/mhtml/).


### XML {#XML}
```
public static final FileType XML
```


XML står för Extensible Markup Language som liknar HTML men skiljer sig åt genom att använda taggar för att definiera objekt. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/xml/).


### MD {#MD}
```
public static final FileType MD
```


Textfiler skapade med Markdown‑språkdialekter sparas med filändelsen .MD eller .MARKDOWN. Läs mer om detta filformat [här](../https://wiki.fileformat.com/word-processing/md/).


### FB2 {#FB2}
```
public static final FileType FB2
```


Filer med FB2‑tillägg är FictionBook 2.0‑e‑bokfiler som innehåller e‑bokens struktur. Läs mer om detta filformat [här](../https://wiki.fileformat.com/ebook/fb2/).


### CHM {#CHM}
```
public static final FileType CHM
```


CHM‑filformatet representerar Microsoft HTML-hjälpfil som består av en samling HTML‑sidor. Läs mer om detta filformat [här](../https://wiki.fileformat.com/web/chm/).


### EPUB {#EPUB}
```
public static final FileType EPUB
```


Filer med .EPUB‑tillägg är ett e‑bokfilformat som tillhandahåller ett standardiserat digitalt publiceringsformat för utgivare och konsumenter. Läs mer om detta filformat [här](../https://wiki.fileformat.com/ebook/epub/).


### AZW3 {#AZW3}
```
public static final FileType AZW3
```


AZW3, även känt som Kindle Format 8 (KF8), är den modifierade versionen av AZW‑e‑bokfilformatet som utvecklats för Amazon Kindle‑enheter. Läs mer om detta filformat [här](../https://wiki.fileformat.com/ebook/azw3/).


### MOBI {#MOBI}
```
public static final FileType MOBI
```


Mobipocket‑filformatet (ursprungligen med filändelsen .prc och senare .mobi) är ett proprietärt, delvis dokumenterat binärt format för e‑böcker. Läs mer om detta filformat [här](../https://wiki.fileformat.com/ebook/mobi/).


### XLS {#XLS}
```
public static final FileType XLS
```


Filer med XLS‑tillägg representerar Excel Binary File Format. Sådana filer kan skapas av Microsoft Excel såväl som andra liknande kalkylprogram som OpenOffice Calc eller Apple Numbers. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xls/).


### XLSX {#XLSX}
```
public static final FileType XLSX
```


XLSX är ett välkänt format för Microsoft Excel‑dokument som introducerades av Microsoft med lanseringen av Microsoft Office 2007. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xlsx/).


### XLSM {#XLSM}
```
public static final FileType XLSM
```


Filer med XLSM‑tillägg är en typ av kalkylbladsfiler som stöder makron. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xlsm/).


### XLSB {#XLSB}
```
public static final FileType XLSB
```


XLSB-filformatet specificerar Excel Binary File Format, som är en samling av poster och strukturer som specificerar innehållet i en Excel-arbetsbok. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xlsb/).


### XLT {#XLT}
```
public static final FileType XLT
```


Filer med .XLT‑tillägget är mallfiler som skapats med Microsoft Excel, som är ett kalkylbladsprogram som ingår i Microsoft Office‑sviten. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xlt/).


### XLTX {#XLTX}
```
public static final FileType XLTX
```


Filer med XLTX‑tillägget representerar Microsoft Excel‑mallfiler som är baserade på Office OpenXML‑filformatspecifikationerna. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xltx/).


### XLTM {#XLTM}
```
public static final FileType XLTM
```


XLTM‑filändelsen representerar filer som genereras av Microsoft Excel som makroaktiverade mallfiler. Läs mer om detta filformat [här](../https://wiki.fileformat.com/specification/spreadsheet/xltm/).


### XLA {#XLA}
```
public static final FileType XLA
```


Excel 97-2003‑tillägget, ett kompletterande program som är avsett att köra extra kod. Stöder användning av VBA‑projekt.


### XLAM {#XLAM}
```
public static final FileType XLAM
```


Det XML‑baserade och makroaktiverade tilläggsformatet för Excel 2010 och Excel 2007. Ett tillägg är ett kompletterande program som är avsett att köra extra kod. Stöder användning av VBA‑projekt och Excel 4.0‑makroblad (.xlm).


### CSV {#CSV}
```
public static final FileType CSV
```


Filer med CSV‑tillägget (Comma Separated Values) representerar rena textfiler som innehåller dataposter med kommaseparerade värden. Läs mer om detta filformat [här](../https://wiki.fileformat.com/spreadsheet/csv/).


### TSV {#TSV}
```
public static final FileType TSV
```


Ett Tab‑Separated Values‑format (TSV) representerar data separerade med tabbar i rent textformat. Läs mer om detta filformat [här](../https://wiki.fileformat.com/spreadsheet/tsv/).


### ODS {#ODS}
```
public static final FileType ODS
```


Filer med ODS‑tillägget står för OpenDocument Spreadsheet‑dokumentformat som kan redigeras av användaren. Läs mer om detta filformat [här](../https://wiki.fileformat.com/spreadsheet/ods/).


### OTS {#OTS}
```
public static final FileType OTS
```


OTS‑filerna innehåller mallfiler som används av OpenOffice‑kalkylprogrammet.


### NUMBERS {#NUMBERS}
```
public static final FileType NUMBERS
```


Filer med .numbers‑filändelse är filer som skapats av Apple iWork Numbers‑kalkylprogrammet.


### PPT {#PPT}
```
public static final FileType PPT
```


En fil med PPT‑tillägget representerar en PowerPoint‑fil som består av en samling bilder för visning som bildspel. Den specificerar det binära filformatet som används av Microsoft PowerPoint 97‑2003. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/ppt/).


### PPTX {#PPTX}
```
public static final FileType PPTX
```


Filer med PPTX‑tillägget är presentationsfiler skapade med det populära Microsoft PowerPoint‑programmet. Till skillnad från den tidigare versionen av presentationsfilformatet PPT som var binärt, är PPTX‑formatet baserat på Microsoft PowerPoint open XML‑presentationsfilformat. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/pptx/).


### PPS {#PPS}
```
public static final FileType PPS
```


PPS‑, PowerPoint Slide Show‑, filer skapas med Microsoft PowerPoint för bildspelsändamål. Läsning och skapande av PPS‑filer stöds av Microsoft PowerPoint 97‑2003. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/pps/).


### PPSX {#PPSX}
```
public static final FileType PPSX
```


PPSX‑, Power Point Slide Show‑, filer skapas med Microsoft PowerPoint 2007 och senare för bildspelsändamål. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/ppsx/).


### ODP {#ODP}
```
public static final FileType ODP
```


Filer med ODP‑extension representerar presentationsfilformat som används av OpenOffice.org i OASISOpen‑standarden. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/odp/).


### POT {#POT}
```
public static final FileType POT
```


Filer med .POT‑extension representerar Microsoft PowerPoint‑mallfiler som skapats av PowerPoint‑versionerna 97‑2003. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/pot/).


### PPTM {#PPTM}
```
public static final FileType PPTM
```


Filer med PPTM‑extension är makroaktiverade presentationsfiler som skapats med Microsoft PowerPoint 2007 eller senare versioner. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/pptm/).


### POTX {#POTX}
```
public static final FileType POTX
```


Filer med .POTX‑extension representerar Microsoft PowerPoint‑mallpresentationer som skapats med Microsoft PowerPoint 2007 och senare. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/potx/).


### POTM {#POTM}
```
public static final FileType POTM
```


Filer med POTM‑extension är Microsoft PowerPoint‑mallfiler med stöd för makron. POTM‑filer skapas med PowerPoint 2007 eller senare och innehåller standardinställningar som kan användas för att skapa ytterligare presentationsfiler. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/potm/).


### PPSM {#PPSM}
```
public static final FileType PPSM
```


Filer med PPSM‑extension representerar makroaktiverade bildspelsfilformat som skapats med Microsoft PowerPoint 2007 eller senare. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/ppsm/).


### OTP {#OTP}
```
public static final FileType OTP
```


Filer med .OTP‑extension representerar presentationsmallfiler som skapats av program i OASIS OpenDocument‑standardformatet. Läs mer om detta filformat [här](../https://wiki.fileformat.com/presentation/otp/).


### MSG {#MSG}
```
public static final FileType MSG
```


MSG är ett filformat som används av Microsoft Outlook och Exchange för att lagra e‑postmeddelanden, kontakter, möten eller andra uppgifter. Läs mer om detta filformat [här](../https://wiki.fileformat.com/email/msg/).


### EML {#EML}
```
public static final FileType EML
```


EML‑filformatet representerar e‑postmeddelanden som sparats med Outlook och andra relevanta program. Läs mer om detta filformat [här](../https://wiki.fileformat.com/email/eml/).


### EMLX {#EMLX}
```
public static final FileType EMLX
```


EMLX‑filformatet är implementerat och utvecklat av Apple. Apple Mail‑programmet använder EMLX‑filformatet för att exportera e‑postmeddelanden. Läs mer om detta filformat [här](../https://wiki.fileformat.com/email/emlx/).


### PST {#PST}
```
public static final FileType PST
```


Filer med .PST‑extension representerar Outlook Personal Storage Files (även kallade Personal Storage Table) som lagrar en mängd användarinformation. Läs mer om detta filformat [här](../https://wiki.fileformat.com/email/pst/).


### OST {#OST}
```
public static final FileType OST
```


OST‑ eller Offline Storage Files representerar användarens brevlådedata i off‑lineläge på den lokala maskinen efter registrering med Exchange Server via Microsoft Outlook. Läs mer om detta filformat [här](../https://wiki.fileformat.com/email/ost/).


### ONE {#ONE}
```
public static final FileType ONE
```


Filer med .ONE‑extension skapas av Microsoft OneNote‑programmet. Läs mer om detta filformat [här](../https://wiki.fileformat.com/note-taking/one/).


### ZIP {#ZIP}
```
public static final FileType ZIP
```


ZIP‑fil‑extension representerar arkiv som kan innehålla en eller flera filer eller kataloger. Läs mer om detta filformat [här](../https://wiki.fileformat.com/compression/zip/).


### SEVENZ {#SEVENZ}
```
public static final FileType SEVENZ
```


7z är ett arkiveringsformat för att komprimera filer och mappar med en hög komprimeringsgrad. Läs mer om detta filformat [här](../https://wiki.fileformat.com/compression/7z/).


### RAR {#RAR}
```
public static final FileType RAR
```


Filer med .rar‑tillägg representerar arkivfiler som skapas för att lagra information i komprimerad eller normal form. Läs mer om detta filformat [här](../https://wiki.fileformat.com/compression/rar/).


### TAR {#TAR}
```
public static final FileType TAR
```


Filer med .tar‑tillägg är arkiv som skapats med ett Unix‑baserat verktyg för att samla en eller flera filer. Läs mer om detta filformat [här](../https://wiki.fileformat.com/compression/tar/).


### GZ {#GZ}
```
public static final FileType GZ
```


Filer med .gz‑tillägg är komprimerade filer som skapats med gzip‑komprimeringsprogrammet. Läs mer om detta filformat [här](../https://wiki.fileformat.com/compression/gz/).


### BZ2 {#BZ2}
```
public static final FileType BZ2
```


Komprimerad fil med Bzip2‑algoritmen.


### TIF {#TIF}
```
public static final FileType TIF
```


TIF, Tagged Image File Format, representerar rasterbilder som är avsedda för användning på en mängd olika enheter som följer denna filformatstandard. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/tiff/).


### TIFF {#TIFF}
```
public static final FileType TIFF
```


TIFF, Tagged Image File Format, representerar rasterbilder som är avsedda för användning på en mängd olika enheter som följer denna filformatstandard. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/tiff/).


### JPG {#JPG}
```
public static final FileType JPG
```


En JPG är en typ av bildformat som sparas med metoden för förlustkomprimering. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jpeg/).


### JPEG {#JPEG}
```
public static final FileType JPEG
```


En JPEG är en typ av bildformat som sparas med metoden för förlustkomprimering. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jpeg/).


### PNG {#PNG}
```
public static final FileType PNG
```


PNG, Portable Network Graphics, avser en typ av rasterbildfilformat som använder förlustfri komprimering. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/png/).


### GIF {#GIF}
```
public static final FileType GIF
```


En GIF eller Graphical Interchange Format är en typ av starkt komprimerad bild. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/gif/).


### BMP {#BMP}
```
public static final FileType BMP
```


Filer med .BMP‑tillägg representerar Bitmap Image‑filer som används för att lagra bitmap‑digitala bilder. Dessa bilder är oberoende av grafikadapter och kallas även device independent bitmap (DIB)‑filformat. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/bmp/).


### ICO {#ICO}
```
public static final FileType ICO
```


Filer med ICO‑tillägg är bildfiltyper som används som ikon för att representera ett program på Microsoft Windows. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/ico/).


### JP2 {#JP2}
```
public static final FileType JP2
```


JPEG 2000 (JP2) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### JPF {#JPF}
```
public static final FileType JPF
```


JPEG 2000 (JPF) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad med vågformsteknik kan JPEG 2000 koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### JPX {#JPX}
```
public static final FileType JPX
```


JPEG 2000 (JPX) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad med vågformsteknik kan JPEG 2000 koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### JPM {#JPM}
```
public static final FileType JPM
```


JPEG 2000 (JPM) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad med vågformsteknik kan JPEG 2000 koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### J2C {#J2C}
```
public static final FileType J2C
```


JPEG 2000 (J2C) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad med vågformsteknik kan JPEG 2000 koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### J2K {#J2K}
```
public static final FileType J2K
```


JPEG 2000 (J2K) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad med vågformsteknik kan JPEG 2000 koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### JPC {#JPC}
```
public static final FileType JPC
```


JPEG 2000 (JPC) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad med vågformsteknik kan JPEG 2000 koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/jp2/).


### DIB {#DIB}
```
public static final FileType DIB
```


En DIB (Device Independent Bitmap)-fil är en rasterbildfil som är liknande i struktur till standard-Bitmap-filer (BMP) men har ett annat huvud. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/dib/).


### WMF {#WMF}
```
public static final FileType WMF
```


Filer med WMF-extension representerar Microsoft Windows Metafile (WMF) för lagring av både vektor- och bitmap-format bilddata. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/wmf/).


### EMF {#EMF}
```
public static final FileType EMF
```


Enhanced metafile format (EMF) lagrar grafiska bilder enhetsoberoende. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/emf/).


### WEBP {#WEBP}
```
public static final FileType WEBP
```


WebP, introducerat av Google, är ett modernt rasterwebb-bildfilformat som bygger på förlustfri och förlustkomprimering. Det ger samma bildkvalitet samtidigt som det avsevärt minskar bildstorleken. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/webp/).


### DJVU {#DJVU}
```
public static final FileType DJVU
```


DjVu är ett grafikfilformat avsett för skannade dokument och böcker, särskilt de som innehåller en kombination av text, teckningar, bilder och fotografier. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/djvu/).


### CGM {#CGM}
```
public static final FileType CGM
```


Computer Graphics Metafile (CGM) är ett fritt, plattformsoberoende, internationellt standardmetafilformat för lagring och utbyte av vektorgrafik (2D), rastergrafik och text. Läs mer om detta filformat [här](../https://wiki.fileformat.com/page-description-language/cgm/).


### PCL {#PCL}
```
public static final FileType PCL
```


PCL står för Printer Command Language, vilket är ett Page Description Language introducerat av Hewlett Packard (HP). Läs mer om detta filformat [här](../https://wiki.fileformat.com/page-description-language/pcl/).


### PSD {#PSD}
```
public static final FileType PSD
```


PSD, Photoshop Document, representerar Adobe Photoshop's inhemska filformat som används för grafisk design och utveckling. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/psd/).


### DCM {#DCM}
```
public static final FileType DCM
```


Filer med .DCM-extension representerar digitala bilder som lagrar medicinsk information om patienter, såsom MR-bilder, CT-skanningar och ultraljudsbilder. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/dcm/).


### PS {#PS}
```
public static final FileType PS
```


PostScript (PS) är ett allmänt syftande sidbeskrivningsspråk som används inom skrivbords- och elektronisk publicering. Läs mer om detta filformat [här](../https://wiki.fileformat.com/page-description-language/ps/).


### EPS {#EPS}
```
public static final FileType EPS
```


Filer med EPS‑tillägg beskriver i huvudsak ett Encapsulated PostScript‑program som beskriver utseendet på en enskild sida. Läs mer om detta filformat [här](../https://wiki.fileformat.com/page-description-language/eps/).


### ODG {#ODG}
```
public static final FileType ODG
```


ODG‑filformatet används av Apache OpenOffice's Draw‑applikationen för att lagra ritningskomponenter som en vektorbild. Läs mer om detta filformat [här](../https://wiki.fileformat.com/image/odg/).


### SVG {#SVG}
```
public static final FileType SVG
```


En SVG‑fil är en Scalar Vector Graphics‑fil som använder ett XML‑baserat textformat för att beskriva en bilds utseende. Läs mer om detta filformat [här](../https://wiki.fileformat.com/page-description-language/svg/).


### PICT {#PICT}
```
public static final FileType PICT
```


PICT‑filformatet är ett meta‑format som kan användas för både bitmap‑bilder och vektor‑bilder.


### getFileFormat() {#getFileFormat--}
```
public String getFileFormat()
```


Filtypnamn t.ex. "Microsoft Word Document".


**Returns:**
java.lang.String – Sträng som representerar en filtyp.

### getExtension() {#getExtension--}
```
public String getExtension()
```


Filnamnsuffix (inklusive punkten ".") t.ex. ".doc".


**Returns:**
java.lang.String – Sträng som representerar en filändelse (inklusive punkten ".").

### getFormat() {#getFormat--}
```
public FileFormat getFormat()
```


Filformat t.ex. "WordProcessing".


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - A member of [FileFormat](../../com.groupdocs.parser.options/fileformat) enum that represents the format of the file.

### equals(Object object) {#equals-java.lang.Object-}
```
public boolean equals(Object object)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Kopplar filändelse till filtyp.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | utökning | java.lang.String | Filändelse (inklusive punkten "."). |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - When file type is supported returns it, otherwise returns default [Unknown](../../com.groupdocs.parser.options/filetype#Unknown) file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Hämtar stödjade filtyper.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.options.FileType> – Returnerar en sekvens av stödda filtyper

