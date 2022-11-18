---
title: FileType
second_title: GroupDocs.Parser för .NET API-referens
description: Representerar filtypen. Ger metoder för att få en lista över alla filtyper som stöds avGroupDocs.Parser .
type: docs
weight: 360
url: /sv/net/groupdocs.parser.options/filetype/
---
## FileType class

Representerar filtypen. Ger metoder för att få en lista över alla filtyper som stöds av**GroupDocs.Parser** .

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | Filnamnssuffix (inklusive perioden ".") t.ex. ".doc". |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | Filtypsnamn t.ex. "Microsoft Word Document". |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | Filformatet t.ex. "WordProcessing". |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | Mappar filtillägget till filtyp. |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | Bestämmer om strömmen[`FileType`](../filetype) är samma som specificerat[`FileType`](../filetype) objekt. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | Bestämmer om strömmen[`FileType`](../filetype) är samma som specificerat objekt. |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | Returnerar hashkoden för den aktuella[`FileType`](../filetype) objekt. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | Returnerar en sträng som representerar det aktuella objektet. |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | Hämtar filtyper som stöds |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | Bestämmer om två[`FileType`](../filetype) objekten är desamma. |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | Bestämmer om två[`FileType`](../filetype) objekt är inte samma sak. |

## Fält

| namn | Beskrivning |
| --- | --- |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | Filer med filtillägget .BMP representerar bitmappsbildfiler som används för att lagra digitala bitmappsbilder. Dessa bilder är oberoende av grafikkort och kallas även enhetsoberoende bitmapp (DIB) file -format. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/bmp/) . |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | Komprimerad fil med Bzip2-algoritmen. |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile (CGM) är gratis, plattformsoberoende, internationell standard metafile -format för lagring och utbyte av vektorgrafik (2D), rastergrafik och text. Läs mer om detta filformat [här](https://wiki.fileformat.com/page-description-language/cgm/) . |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM-filformatet representerar Microsoft HTML-hjälpfil som består av en samling HTML-sidor. Läs mer om detta filformat [här](https://wiki.fileformat.com/web/chm/) . |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | Filer med tillägget CSV (Comma Separated Values) representerar vanliga textfiler som innehåller dataposter med kommaseparerade värden. Läs mer om detta filformat [här](https://wiki.fileformat.com/spreadsheet/csv/) . |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | Filer med filtillägget .DCM representerar en digital bild som lagrar medicinsk information om patienter såsom MRI, datortomografi och ultraljudsbilder. Läs mer om detta filformat [här](https://wiki.fileformat.com/image/dcm/) . |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | En DIB-fil (Device Independent Bitmap) är en rasterbildsfil som i strukturen liknar standardbitmappsfilerna (BMP) men har en annan rubrik. Lär dig mer om detta filformat [här](https://wiki.fileformat.com/image/dib/) . |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu, uttalas som "déjà vu", är ett grafikfilformat avsett för skannade dokument och böcker, särskilt de som innehåller en kombination av text, teckningar, bilder och fotografier. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/djvu/) . |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | Filer med filtillägget .doc representerar dokument som genererats av Microsoft Word eller andra ordbehandlingsdokument i binärt filformat. Läs mer om detta filformat [här](https://wiki.fileformat.com/word-processing/doc/) . |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM-filer är Microsoft Word 2007 eller högre genererade dokument med möjlighet att köra makron. Läs mer om detta filformat[här](https://wiki.fileformat.com/word-processing/docm/) . |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX är ett välkänt format för Microsoft Word-dokument. Introducerad från 2007 med release av Microsoft Office 2007, ändrades strukturen för detta nya dokumentformat från vanlig binary till en kombination av XML och binära filer. Läs mer om detta filformat [här](https://wiki.fileformat.com/word-processing/docx/) . |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | Filer med filtillägget .DOT är mallfiler skapade av Microsoft Word för att ha förformaterade settings för generering av ytterligare DOC- eller DOCX-filer. Läs mer om detta filformat [här](https://wiki.fileformat.com/word-processing/dot/) . |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | En fil med DOTM-tillägget representerar en mallfil skapad med Microsoft Word 2007 eller högre. Läs mer om detta filformat[här](https://wiki.fileformat.com/word-processing/dotm/) . |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | Filer med DOTX-tillägg är mallfiler skapade av Microsoft Word för att ha förformaterade settings för generering av ytterligare DOCX-filer. Läs mer om detta filformat [här](https://wiki.fileformat.com/word-processing/dotx/) . |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | Enhanced metafile format (EMF) lagrar grafiska bilder enhetsoberoende. Läs mer om detta filformat [här](https://wiki.fileformat.com/image/emf/) . |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML-filformat representerar e-postmeddelanden som sparats med Outlook och andra relevanta applikationer. Läs mer om detta filformat[här](https://wiki.fileformat.com/email/eml/) . |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX-filformatet är implementerat och utvecklat av Apple. Apple Mail-applikationen använder filformatet EMLX för att exportera e-postmeddelanden. Läs mer om detta filformat [här](https://wiki.fileformat.com/email/emlx/) . |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | Filer med EPS-tillägg beskriver i huvudsak ett Encapsulated PostScript-språkprogram som beskriver utseendet på en enda sida. Läs mer om detta filformat [här](https://wiki.fileformat.com/page-description-language/eps/) . |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | Filer med filtillägget .EPUB är ett e-boksfilformat som tillhandahåller ett standardformat digitalt publikationsformat för förlag och konsumenter. Läs mer om detta filformat [här](https://wiki.fileformat.com/ebook/epub/) . |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | Filer med tillägg FB2 är FictionBook 2.0 eBook-filer som innehåller e-bokens struktur. Läs mer om detta filformat [här](https://wiki.fileformat.com/ebook/fb2/) . |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | En GIF eller Graphical Interchange Format är en typ av mycket komprimerad bild. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/gif/) . |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | Filer med filtillägget .gz är komprimerade filer som skapats med gzip-komprimeringsprogrammet. Läs mer om detta filformat [här](https://wiki.fileformat.com/compression/gz/) . |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | Filer med HTM-tillägg representerar Hypertext Markup Language för att skapa webbsidor för visning i webbläsare som Google Chrome, Internet Explorer, Firefox och ett antal andra. Läs mer om detta filformat [här](https://wiki.fileformat.com/web/htm/) . |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML (Hyper Text Markup Language) är tillägget för webbsidor som skapats för visning i webbläsare. Läs mer om detta filformat [här](https://wiki.fileformat.com/web/html/) . |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | Filer med tillägget ICO är bildfiltyper som används som ikon för representation av ett program på Microsoft Windows. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/ico/) . |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000 (J2C) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad, med hjälp av wavelet-teknik JPEG 2000 kan koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000 (J2K) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad, med hjälp av wavelet-teknik JPEG 2000 kan koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000 (JP2) är ett bildkodningssystem och toppmodern bildkomprimeringsstandard. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000 (JPC) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad, med hjälp av wavelet-teknik JPEG 2000 kan koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | En JPEG är en typ av bildformat som sparas med metoden för förlustkomprimering. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jpeg/) . |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000 (JPF) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad, med hjälp av wavelet-teknik JPEG 2000 kan koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | En JPG är en typ av bildformat som sparas med metoden för förlustkomprimering. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jpeg/) . |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad, med hjälp av wavelet-teknik JPEG 2000 kan koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) är ett bildkodningssystem och en toppmodern bildkomprimeringsstandard. Designad, med hjälp av wavelet-teknik JPEG 2000 kan koda förlustfritt innehåll i vilken kvalitet som helst på en gång. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | Textfiler skapade med Markdown-språkdialekter sparas med filtillägget .MD eller .MARKDOWN. Lär dig mer om detta filformat [här](https://wiki.fileformat.com/word-processing/md/) . |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | Filer med MHT-tillägg representerar ett webbsidearkivformat som kan skapas av ett antal olika applikationer. Lär dig mer om detta filformat [här](https://wiki.fileformat.com/web/mhtml/) . |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | Filer med MHTML-tillägg representerar ett webbsidearkivformat som kan skapas av ett antal olika applikationer. Lär dig mer om detta filformat [här](https://wiki.fileformat.com/web/mhtml/) . |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG är ett filformat som används av Microsoft Outlook och Exchange för att lagra e-postmeddelanden, kontakt, möte eller andra uppgifter. Läs mer om detta filformat [här](https://wiki.fileformat.com/email/msg/) . |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | Filer som innehåller filtillägget .numbers är filer som skapas av kalkylarksprogrammet Apple iWork Numbers. |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | ODG-filformatet används av Apache OpenOffices Draw-applikation för att lagra ritelement som en vektorbild. Läs mer om detta filformat [här](https://wiki.fileformat.com/image/odg/) . |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | Filer med ODP-tillägg representerar presentationsfilformat som används av OpenOffice.org i OASISOpen-standarden. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/odp/) . |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | Filer med ODS-tillägg står för OpenDocument Spreadsheet Document-format som kan redigeras av användaren. Läs mer om detta filformat [här](https://wiki.fileformat.com/spreadsheet/ods/) . |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT-filer är typ av dokument skapade med ordbehandlingsprogram som är baserade på OpenDocument Text File-format. Dessa skapas med ordbehandlingsprogram som gratis OpenOffice Writer och kan innehålla innehåll som text, bilder, objekt och stilar. Läs mer om detta filformat [här](https://wiki.fileformat.com/word-processing/odt/) . |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | Filer som representeras av .ONE-tillägget skapas av Microsoft OneNote-applikationen. Läs mer om detta filformat [här](https://wiki.fileformat.com/note-taking/one/) . |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST eller offlinelagringsfiler representerar användarens postlådedata i offlineläge på lokal dator vid registrering med Exchange Server som använder Microsoft Outlook. Läs mer om detta filformat [här](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | Filer med tillägget .OTP representerar presentationsmallfiler skapade av applikationer i OASIS OpenDocument standardformat. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/otp/) . |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS-filerna innehåller mallfiler som används av OpenOffice-kalkylprogrammet. |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | Filer med OTT-tillägg representerar malldokument som genereras av applikationer i enlighet med OASIS OpenDocument-standardformat. Läs mer om detta filformat [här](https://wiki.fileformat.com/word-processing/ott/) . |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL står för Printer Command Language som är ett Page Description Language som introducerats av Hewlett Packard (HP). Läs mer om detta filformat [här](https://wiki.fileformat.com/page-description-language/pcl/) . |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | Portable Document Format (PDF) är en typ av dokument som skapades av Adobe redan på 1990-talet. Syftet med detta filformat var att införa en standard för representation av dokument och annat referensmaterial i ett format som är oberoende av applikationsprogramvara, hårdvara samt operativsystem. Läs mer om detta filformat[här](https://wiki.fileformat.com/view/pdf/) . |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT-filformatet är ett metaformat som kan användas för både bitmappsbilder och vektorbilder. |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG, Portable Network Graphics, hänvisar till en typ av rasterbildsfilformat som använder förlustfri komprimering. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/png/) . |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | Filer med tillägget .POT representerar Microsoft PowerPoint-mallfiler skapade av PowerPoint 97-2003-versioner. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/pot/) . |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | Filer med POTM-tillägg är Microsoft PowerPoint-mallfiler med stöd för makron. POTM-filer skapas med PowerPoint 2007 eller senare och innehåller standardinställningar som kan användas för att skapa ytterligare presentationsfiler. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/potm/) . |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | Filer med tillägget .POTX representerar Microsoft PowerPoint-mallpresentationer som skapas med Microsoft PowerPoint 2007 och senare. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/potx/) . |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS, PowerPoint Slide Show, filer skapas med Microsoft PowerPoint för Slide Show-ändamål. Läsning och skapande av PPS-filer stöds av Microsoft PowerPoint 97-2003. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/pps/) . |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | Filer med PPSM-tillägget representerar Macro-aktiverat bildspelsfilformat som skapats med Microsoft PowerPoint 2007 eller högre. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/ppsm/) . |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX, Power Point Slide Show, filen skapas med Microsoft PowerPoint 2007 och högre för Slide Show syfte. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/ppsx/) . |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | En fil med PPT-tillägg representerar en PowerPoint-fil som består av en samling bilder för som visas som bildspel. Den anger det binära filformatet som används av Microsoft PowerPoint 97-2003. Läs mer om detta filformat[här](https://wiki.fileformat.com/presentation/ppt/) . |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | Filer med PPTM-tillägg är makroaktiverade presentationsfiler som skapas med Microsoft PowerPoint 2007 eller högre versioner. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/pptm/) . |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | Filer med PPTX-tillägg är presentationsfiler skapade med populära Microsoft PowerPoint-applikation. Till skillnad från den tidigare versionen av presentationsfilformatet PPT som var binärt, är PPTX-formatet baserat på Microsoft PowerPoints öppna XML-presentationsfilformat. Läs mer om detta filformat [här](https://wiki.fileformat.com/presentation/pptx/) . |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) är ett allmänt sidbeskrivningsspråk som används i branschen för desktop och elektronisk publicering. Läs mer om detta filformat [här](https://wiki.fileformat.com/page-description-language/ps/) . |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD, Photoshop Document, representerar Adobe Photoshops ursprungliga filformat som används för grafisk design och utveckling. Läs mer om detta filformat [här](https://wiki.fileformat.com/image/psd/) . |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | Filer med tillägget .PST representerar Outlook Personal Storage Files (även kallad Personal Storage Table) som lagrar en mängd olika användarinformation. Läs mer om detta filformat [här](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | Filer med tillägget .rar representerar arkivfiler som skapats för att lagra information i komprimerad eller normal form. Läs mer om detta filformat [här](https://wiki.fileformat.com/compression/rar/) . |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | Introducerat och dokumenterat av Microsoft, Rich Text Format (RTF) representerar en metod för att koda formaterad text och grafik för användning i applikationer. Formatet underlättar plattformsoberoende dokument utbyte med andra Microsoft-produkter, vilket tjänar syftet med interoperabilitet. Läs mer om detta filformat[här](https://wiki.fileformat.com/word-processing/rtf/) . |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z är ett arkiveringsformat för att komprimera filer och mappar med ett högt komprimeringsförhållande. Läs mer om detta filformat [här](https://wiki.fileformat.com/compression/7z/) . |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | En SVG-fil är en Scalar Vector Graphics-fil som använder XML-baserat textformat för att beskriva utseendet på en bild. Läs mer om detta filformat [här](https://wiki.fileformat.com/page-description-language/svg/) . |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | Filer med tillägget .tar är arkiv skapade med Unix-baserat verktyg för att samla in en eller flera filer. Läs mer om detta filformat [här](https://wiki.fileformat.com/compression/tar/) . |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | En fil med tillägget .TEXT representerar ett textdokument som innehåller ren text i form av rader. Läs mer om detta filformat[här](https://wiki.fileformat.com/word-processing/txt/) . |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF, Tagged Image File Format, representerar rasterbilder som är avsedda för användning på en mängd av enheter som överensstämmer med denna filformatstandard. Läs mer om detta filformat [här](https://wiki.fileformat.com/image/tiff/) . |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF, Tagged Image File Format, representerar rasterbilder som är avsedda för användning på en mängd av enheter som överensstämmer med denna filformatstandard. Läs mer om detta filformat [här](https://wiki.fileformat.com/image/tiff/) . |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | Ett TSV-filformat (Tab-Separated Values) representerar data separerade med flikar i vanlig textformat. Läs mer om detta filformat [här](https://wiki.fileformat.com/spreadsheet/tsv/) . |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | En fil med filtillägget .TXT representerar ett textdokument som innehåller vanlig text i form av rader. Läs mer om detta filformat[här](https://wiki.fileformat.com/word-processing/txt/) . |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | Representerar okänd filtyp. |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP, introducerat av Google, är ett modernt rasterwebbbildfilformat som är baserat på förlustfri och förlustfri komprimering. Den ger samma bildkvalitet samtidigt som den minskar bildstorleken avsevärt. Läs mer om detta filformat[här](https://wiki.fileformat.com/image/webp/) . |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | Filer med WMF-tillägg representerar Microsoft Windows Metafile (WMF) för lagring av vektor samt bilddata i bitmappsformat. Lär dig mer om detta filformat [här](https://wiki.fileformat.com/image/wmf/) . |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML är ett textbaserat filformat med markering i XML, med en omformulering av HTML 4.0. Läs mer om detta filformat [här](https://wiki.fileformat.com/web/xhtml/) . |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | Excel 97-2003-tillägget, ett tilläggsprogram som är utformat för att köra ytterligare kod. Stöder användningen av VBA-projekt. |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | Det XML-baserade och makroaktiverade tilläggsformatet för Excel 2010 och Excel 2007. Ett tillägg är ett tilläggsprogram som är utformat för att köra ytterligare kod. Stöder användningen av VBA-projekt och Excel 4.0 makroblad (.xlm). |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | Filer med XLS-tillägg representerar det binära filformatet i Excel. Sådana filer kan skapas av Microsoft Excel såväl som andra liknande kalkylprogram som OpenOffice Calc eller Apple Numbers. Läs mer om detta filformat[här](https://wiki.fileformat.com/specification/spreadsheet/xls/) . |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB-filformatet anger det binära filformatet för Excel, som är en samling poster och strukturer som anger innehållet i Excel-arbetsboken. Läs mer om detta filformat [här](https://wiki.fileformat.com/specification/spreadsheet/xlsb/) . |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | Filer med tillägget XLSM är en typ av kalkylbladsfiler som stöder makron. Läs mer om detta filformat [här](https://wiki.fileformat.com/specification/spreadsheet/xlsm/) . |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX är ett välkänt format för Microsoft Excel-dokument som introducerades av Microsoft med release av Microsoft Office 2007. Läs mer om detta filformat [här](https://wiki.fileformat.com/specification/spreadsheet/xlsx/) . |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | Filer med filtillägget .XLT är mallfiler skapade med Microsoft Excel som är ett kalkylblad -program som kommer som en del av Microsoft Office-paketet. Läs mer om detta filformat [här](https://wiki.fileformat.com/specification/spreadsheet/xlt/) . |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | Filtillägget XLTM representerar filer som genereras av Microsoft Excel som Macro-enabled mallfiler. Läs mer om detta filformat [här](https://wiki.fileformat.com/specification/spreadsheet/xltm/) . |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | Filer med tillägget XLTX representerar Microsoft Excel-mallfiler som är baserade på Office OpenXML filformatspecifikationer. Läs mer om detta filformat [här](https://wiki.fileformat.com/specification/spreadsheet/xltx/) . |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML står för Extensible Markup Language som liknar HTML men skiljer sig från att använda taggar för att definiera objekt. Lär dig mer om detta filformat [här](https://wiki.fileformat.com/web/xml/) . |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP-filtillägget representerar arkiv som kan innehålla en eller flera filer eller kataloger. Läs mer om detta filformat [här](https://wiki.fileformat.com/compression/zip/) . |

### Anmärkningar

**Läs mer:**

* [Dokumentformat som stöds](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [Få filformat som stöds](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [Få dokumentinformation](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### Se även

* namnutrymme [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* hopsättning [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
