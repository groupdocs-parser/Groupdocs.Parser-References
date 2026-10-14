---
title: "Parser"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili kelas utama yang mengontrol ekstraksi kontainer gambar teks dan fungsionalitas parsing."
type: docs
weight: 10
url: /id/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Mewakili kelas utama yang mengontrol teks, gambar, ekstraksi kontainer, dan fungsionalitas penguraian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL dengan loadOptions. |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL dengan parserSettings. |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL dengan loadOptions dan parserSettings. |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari basis data. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari basis data. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dan [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dan [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Mengembalikan informasi umum tentang sebuah file. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Mengembalikan informasi umum tentang sebuah file. |
|
|  | [getFeatures()](#getFeatures--) | Mendapatkan fitur yang didukung. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Membuat pratinjau halaman dokumen. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Membuat pratinjau halaman dokumen menggunakan opsi kustomisasi. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Dapatkan pratinjau halaman. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Mengembalikan informasi umum tentang dokumen. |
|
|  | [getText()](#getText--) | Mengekstrak teks dari dokumen. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Mengekstrak halaman teks dari dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah). |
|
|  | [getText(int pageIndex)](#getText-int-) | Mengekstrak teks dari halaman dokumen. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Mengekstrak teks dari halaman dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Mengekstrak teks terformat dari dokumen. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Mengekstrak teks terformat dari halaman dokumen. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Mencari kata kunci dalam dokumen. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Mencari kata kunci dalam dokumen menggunakan opsi pencarian (ekspresi reguler, cocok huruf besar/kecil, dll.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Mengekstrak sorotan dari dokumen. |
|
|  | [getToc()](#getToc--) | Mengekstrak daftar isi dari dokumen. |
|
|  | [getMetadata()](#getMetadata--) | Mengekstrak metadata dari dokumen. |
|
|  | [getAnnotations()](#getAnnotations--) | Mengekstrak anotasi dari dokumen. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Mengekstrak anotasi dari halaman dokumen. |
|
|  | [getContainer()](#getContainer--) | Mengekstrak objek kontainer dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll. |
|
|  | [getTextAreas()](#getTextAreas--) | Mengekstrak area teks dari dokumen. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Mengekstrak area teks dari dokumen menggunakan opsi penyesuaian (ekspresi reguler, cocokkan huruf, dll). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Mengekstrak area teks dari halaman dokumen. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Mengekstrak area teks dari halaman dokumen menggunakan opsi penyesuaian (ekspresi reguler, cocokkan huruf, dll). |
|
|  | [getImages()](#getImages--) | Mengekstrak gambar dari dokumen. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Mengekstrak gambar dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Mengekstrak gambar dari halaman dokumen. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Mengekstrak gambar dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Mengekstrak tautan dari dokumen. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Mengekstrak tautan dari halaman dokumen. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Mengekstrak tautan dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Mengekstrak tautan dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan). |
|
|  | [getBarcodes()](#getBarcodes--) | Mengekstrak kode batang dari dokumen. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Mengekstrak kode batang dari halaman dokumen. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Mengekstrak kode batang dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi kode batang). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Mengekstrak kode batang dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi kode batang). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Mengekstrak tabel dari dokumen. |
|
|  | [getTables()](#getTables--) | Mengekstrak tabel dari dokumen, mendeteksinya secara otomatis. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Mengekstrak tabel dari halaman dokumen. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Mengekstrak tabel dari halaman dokumen, mendeteksinya secara otomatis. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Menghasilkan kumpulan penyesuaian [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s untuk dokumen. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Mengekstrak info tentang semua lembar kerja dalam spreadsheet. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Mengekstrak info tentang lembar kerja. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Mengekstrak sel lembar kerja. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Mengekstrak sel lembar kerja menggunakan opsi penyesuaian. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Menganalisis dokumen dengan templat yang dibuat pengguna. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Menganalisis dokumen dengan templat yang dibuat pengguna menggunakan opsi yang disediakan. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Menganalisis dokumen dengan secara otomatis memilih templat yang paling cocok dari koleksi. |
|
|  | [parseForm()](#parseForm--) | Menganalisis formulir dokumen. |
|
|  | [getStructure()](#getStructure--) | Mengekstrak teks terstruktur dari dokumen. |
|
|  | [close()](#close--) | Menutup sumber daya ini, melepaskan semua sumber daya yang mendasarinya. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | url | java.net.URL | URL tempat permintaan dikirim |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL dengan loadOptions.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | url | java.net.URL | URL tempat permintaan dikirim. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka file. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL dengan parserSettings.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | url | java.net.URL | URL tempat permintaan dikirim. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Menginisialisasi sebuah instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari sebuah URL dengan loadOptions dan parserSettings.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | url | java.net.URL | URL tempat permintaan dikirim. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari basis data.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Contoh berikut menunjukkan cara mengekstrak data dari basis data Sqlite:

````
// Create DbConnection object
 java.sql.Connection connection = java.sql.DriverManager.getConnection(String.format("jdbc:sqlite:%s", Constants.SampleDatabase));
 // Create an instance of Parser class to extract tables from the database
 try (Parser parser = new Parser(connection)) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     // Check if toc extraction is supported
     if (!parser.getFeatures().isToc()) {
         System.out.println("Toc extraction isn't supported.");
         return;
     }
     // Get a list of tables
     Iterable toc = parser.getToc();
     // Iterate over tables
     for(TocItem i : toc)
     {
         // Print the table name
         System.out.println(i.extractText());
         // Extract a table content as a text
         try(TextReader reader = parser.getText(i.getPageIndex().intValue()))
         {
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | koneksi | java.sql.Connection | Koneksi basis data. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) untuk mengekstrak data dari basis data.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Contoh berikut menunjukkan cara mengekstrak data dari basis data Sqlite:

````
// Create DbConnection object
 java.sql.Connection connection = java.sql.DriverManager.getConnection(String.format("jdbc:sqlite:%s", Constants.SampleDatabase));
 // Create an instance of Parser class to extract tables from the database
 try (Parser parser = new Parser(connection)) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     // Check if toc extraction is supported
     if (!parser.getFeatures().isToc()) {
         System.out.println("Toc extraction isn't supported.");
         return;
     }
     // Get a list of tables
     Iterable toc = parser.getToc();
     // Iterate over tables
     for(TocItem i : toc)
     {
         // Print the table name
         System.out.println(i.extractText());
         // Extract a table content as a text
         try(TextReader reader = parser.getText(i.getPageIndex().intValue()))
         {
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | koneksi | java.sql.Connection | Koneksi basis data. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Contoh berikut menunjukkan cara mengekstrak email dari Exchange Server:

````
// Create the connection object for Exchange Web Services protocol
 EmailConnection connection = new EmailEwsConnection(
         "https://outlook.office365.com/ews/exchange.asmx",
         "email@server",
         "password");
 // Create an instance of Parser class to extract emails from the remote server
 try (Parser parser = new Parser(connection)) {
     // Check if container extraction is supported
     if (!parser.getFeatures().isContainer()) {
         System.out.println("Container extraction isn't supported.");
         return;
     }
     // Extract email messages from the server
     Iterable emails = parser.getContainer();
     // Iterate over attachments
     for (ContainerItem item : emails) {
         // Create an instance of Parser class for email message
         try (Parser emailParser = item.openParser()) {
             // Extract the email text
             try (TextReader reader = emailParser.getText()) {
                 // Print the email text
                 System.out.println(reader == null ? "Text extraction isn't supported." : reader.readToEnd());
             }
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Koneksi email. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Contoh berikut menunjukkan cara mengekstrak email dari Exchange Server:

````
// Create the connection object for Exchange Web Services protocol
 EmailConnection connection = new EmailEwsConnection(
         "https://outlook.office365.com/ews/exchange.asmx",
         "email@server",
         "password");
 // Create an instance of Parser class to extract emails from the remote server
 try (Parser parser = new Parser(connection)) {
     // Check if container extraction is supported
     if (!parser.getFeatures().isContainer()) {
         System.out.println("Container extraction isn't supported.");
         return;
     }
     // Extract email messages from the server
     Iterable emails = parser.getContainer();
     // Iterate over attachments
     for (ContainerItem item : emails) {
         // Create an instance of Parser class for email message
         try (Parser emailParser = item.openParser()) {
             // Extract the email text
             try (TextReader reader = emailParser.getText()) {
                 // Print the email text
                 System.out.println(reader == null ? "Text extraction isn't supported." : reader.readToEnd());
             }
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Koneksi email. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Contoh berikut menunjukkan cara memuat dokumen dari disk lokal:

````
// Set the filePath
 String filePath = Constants.SamplePdf;
 // Create an instance of Parser class with the filePath
 try (Parser parser = new Parser(filePath)) {
     // Extract a text into the reader
     try (TextReader reader = parser.getText()) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Kata sandi dokumen diteruskan oleh kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions):

````
try {
     String password = "123456";
     // Create an instance of Parser class with the password:
     try (Parser parser = new Parser(Constants.SamplePassword, new LoadOptions(password))) {
         // Check if text extraction is supported
         if (!parser.getFeatures().isText()) {
             System.out.println("Text extraction isn't supported.");
             return;
         }
         // Print the document text
         try (TextReader reader = parser.getText()) {
             System.out.println(reader.readToEnd());
         }
     }
 } catch (InvalidPasswordException ex) {
     // Print the message if the password is incorrect or empty
     System.out.println("Invalid password");
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka file. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dan [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Contoh berikut menunjukkan cara menerima informasi melalui antarmuka [ILogger](../../com.groupdocs.parser.options/ilogger):

````
try {
     // Create an instance of Logger class
     Logger logger = new Logger();
     // Create an instance of Parser class with the parser settings
     try (Parser parser = new Parser(Constants.SamplePassword, null, new ParserSettings(logger))) {
         // Check if text extraction is supported
         if (!parser.getFeatures().isText()) {
             System.out.println("Text extraction isn't supported.");
             return;
         }
         // Print the document text
         try (TextReader reader = parser.getText()) {
             System.out.println(reader.readToEnd());
         }
     }
 } catch (InvalidPasswordException | IOException ex) {
     ; // Ignore the exception
 }

 class Logger implements ILogger {
     public void error(String message, Exception exception) {
         // Print error message
         System.out.println("Error: " + message);
     }

     public void trace(String message) {
         // Print event message
         System.out.println("Event: " + message);
     }

     public void warning(String message) {
         // Print warning message
         System.out.println("Warning: " + message);
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Contoh berikut menunjukkan cara memuat dokumen dari aliran:

````
// Create the stream
 try (InputStream stream = new FileInputStream(Constants.SamplePdf)) {
     // Create an instance of Parser class with the stream
     try (Parser parser = new Parser(stream)) {
         // Extract a text into the reader
         try (TextReader reader = parser.getText()) {
             // Print a text from the document
             // If text extraction isn't supported, a reader is null
             System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran masukan sumber. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Dalam beberapa kasus diperlukan untuk mendefinisikan [FileFormat](../../com.groupdocs.parser.options/fileformat). Baik untuk kasus khusus (basis data, server email)
dan untuk mendeteksi tipe file berdasarkan kontennya:

````
// Create an instance of Parser class for markdown document
 try (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup))) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     try (TextReader reader = parser.getText()) {
         // Print the document text
         // Markdown is detected; text without special symbols is printed
         System.out.println(reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran masukan sumber. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka file. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran masukan sumber. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Menginisialisasi instance baru dari kelas [Parser](../../com.groupdocs.parser/parser) dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dan [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Contoh berikut menunjukkan cara menerima informasi melalui antarmuka [ILogger](../../com.groupdocs.parser.options/ilogger):

````
try {
     // Create an instance of Logger class
     Logger logger = new Logger();
     // Create an instance of Parser class with the parser settings
     try (Parser parser = new Parser(Constants.SamplePassword, null, new ParserSettings(logger))) {
         // Check if text extraction is supported
         if (!parser.getFeatures().isText()) {
             System.out.println("Text extraction isn't supported.");
             return;
         }
         // Print the document text
         try (TextReader reader = parser.getText()) {
             System.out.println(reader.readToEnd());
         }
     }
 } catch (InvalidPasswordException | IOException ex) {
     ; // Ignore the exception
 }

 class Logger implements ILogger {
     public void error(String message, Exception exception) {
         // Print error message
         System.out.println("Error: " + message);
     }

     public void trace(String message) {
         // Print event message
         System.out.println("Event: " + message);
     }

     public void warning(String message) {
         // Print warning message
         System.out.println("Warning: " + message);
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran masukan sumber. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Mengembalikan informasi umum tentang sebuah file.

Kode berikut menunjukkan cara memeriksa apakah sebuah file dilindungi kata sandi:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Mengembalikan informasi umum tentang sebuah file.

Kode berikut menunjukkan cara memeriksa apakah sebuah file dilindungi kata sandi:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran masukan sumber. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Mendapatkan fitur yang didukung.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Jika fitur tidak didukung, metode mengembalikan
null
alih-alih nilai. Beberapa operasi mungkin memakan
waktu yang signifikan. Jadi tidak optimal memanggil metode hanya untuk memeriksa dukungan fitur.
Untuk tujuan ini properti Features digunakan:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Check if text extraction is supported for the document
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported");
         return;
     }
     // Extract a text from the document
     try (TextReader reader = parser.getText()) {
         System.out.println(reader.readToEnd());
     }
 }
 
````



**Returns:**
[Features](../../com.groupdocs.parser.options/features) - An instance of [Features](../../com.groupdocs.parser.options/features) class that represents the supported features.

### getPagePreview(int pageIndex) {#getPagePreview-int-}
```
public OutputStream getPagePreview(int pageIndex)
```


Membuat pratinjau halaman dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.io.OutputStream - Sebuah instance java.io.OutputStream yang berisi gambar halaman dokumen; null jika pembuatan pratinjau halaman tidak didukung.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Membuat pratinjau halaman dokumen menggunakan opsi kustomisasi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Opsi untuk menyesuaikan pembuatan pratinjau. |
|

**Returns:**
java.io.OutputStream - Sebuah instance java.io.OutputStream yang berisi gambar halaman dokumen; null jika pembuatan pratinjau halaman tidak didukung.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Dapatkan pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Mengembalikan informasi umum tentang dokumen.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Contoh berikut menunjukkan cara mendapatkan informasi dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Get the document info
     IDocumentInfo info = parser.getDocumentInfo();
     // Print document information
     System.out.println(String.format("FileType: %s", info.getFileType()));
     System.out.println(String.format("PageCount: %d", info.getPageCount()));
     System.out.println(String.format("Size: %d", info.getSize()));
 }
 
````



**Returns:**
[IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) - An instance of class that implements [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) interface.

### getText() {#getText--}
```
public TextReader getText()
```


Mengekstrak teks dari dokumen.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Contoh berikut menunjukkan cara mengekstrak teks dari dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a text into the reader
     try (TextReader reader = parser.getText()) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(TextOptions options) {#getText-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(TextOptions options)
```


Mengekstrak halaman teks dari dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Contoh berikut menunjukkan cara mengekstrak teks mentah dari dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a raw text into the reader
     try (TextReader reader = parser.getText(new TextOptions(true))) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Opsi ekstraksi teks. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Mengekstrak teks dari halaman dokumen.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Contoh berikut menunjukkan cara mengekstrak teks dari halaman dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Check if the document supports text extraction
     if (!parser.getFeatures().isText()) {
         System.out.println("Document isn't supports text extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int p = 0; p < documentInfo.getPageCount(); p++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", p + 1, documentInfo.getPageCount()));
         // Extract a text into the reader
         try (TextReader reader = parser.getText(p)) {
             // Print a text from the document
             // We ignore null-checking as we have checked text extraction feature support earlier
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Mengekstrak teks dari halaman dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Contoh berikut menunjukkan cara mengekstrak teks mentah dari halaman dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Check if the document supports text extraction
     if (!parser.getFeatures().isText()) {
         System.out.println("Document isn't supports text extraction.");
         return;
     }
     // Get the document info
     DocumentInfo documentInfo = parser.getDocumentInfo() instanceof DocumentInfo
             ? (DocumentInfo) parser.getDocumentInfo()
             : null;
     // Check if the document has pages
     if (documentInfo == null || documentInfo.getRawPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int p = 0; p < documentInfo.getRawPageCount(); p++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", p + 1, documentInfo.getPageCount()));
         // Extract a text into the reader
         try (TextReader reader = parser.getText(p, new TextOptions(true))) {
             // Print a text from the document
             // We ignore null-checking as we have checked text extraction feature support earlier
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Opsi ekstraksi teks. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Mengekstrak teks terformat dari dokumen.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Contoh berikut menunjukkan cara mengekstrak teks dokumen sebagai teks HTML:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Extract a formatted text into the reader
     try (TextReader reader = parser.getFormattedText(new FormattedTextOptions(FormattedTextMode.Html))) {
         // Print a formatted text from the document
         // If formatted text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Formatted text extraction isn't suppported" : reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Opsi ekstraksi teks terformat. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Mengekstrak teks terformat dari halaman dokumen.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Contoh berikut menunjukkan cara mengekstrak teks halaman dokumen sebagai teks Markdown:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Check if the document supports formatted text extraction
     if (!parser.getFeatures().isFormattedText()) {
         System.out.println("Document isn't supports formatted text extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int p = 0; p < documentInfo.getPageCount(); p++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", p + 1, documentInfo.getPageCount()));
         // Extract a formatted text into the reader
         try (TextReader reader = parser.getFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown))) {
             // Print a formatted text from the document
             // We ignore null-checking as we have checked formatted text extraction feature support earlier
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Opsi ekstraksi teks terformat. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Mencari kata kunci dalam dokumen.

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

Contoh berikut menunjukkan cara menemukan kata kunci dalam dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Search a keyword:
     Iterable sr = parser.search("lorem");
     // Check if search is supported
     if (sr == null) {
         System.out.println("Search isn't supported");
         return;
     }
     // Iterate over search results
     for (SearchResult s : sr) {
         // Print an index and found text:
         System.out.println(String.format("At %d: %s", s.getPosition(), s.getText()));
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata kunci | java.lang.String | Kata kunci untuk pencarian. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Sekumpulan objek [SearchResult](../../com.groupdocs.parser.data/searchresult); null jika pencarian tidak didukung.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Mencari kata kunci dalam dokumen menggunakan opsi pencarian (ekspresi reguler, cocok huruf besar/kecil, dll.).

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

Contoh berikut menunjukkan cara mencari dengan ekspresi reguler dalam dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Search with a regular expression with case matching
     Iterable sr = parser.search("[0-9]+", new SearchOptions(true, false, true));
     // Check if search is supported
     if (sr == null) {
         System.out.println("Search isn't supported");
         return;
     }
     // Iterate over search results
     for (SearchResult s : sr) {
         // Print an index and found text:
         System.out.println(String.format("At %d: %s", s.getPosition(), s.getText()));
     }
 }
 
````

Contoh berikut menunjukkan cara mencari teks pada halaman:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Search a keyword with page numbers
     Iterable sr = parser.search("lorem", new SearchOptions(false, false, false, true));
     // Check if search is supported
     if (sr == null) {
         System.out.println("Search isn't supported");
         return;
     }
     // Iterate over search results
     for (SearchResult s : sr) {
         // Print an index, page number and found text:
         System.out.println(String.format("At %d (%d): %s", s.getPosition(), s.getPageIndex(), s.getText()));
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata kunci | java.lang.String | Kata kunci untuk pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Opsi pencarian. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Sekumpulan objek [SearchResult](../../com.groupdocs.parser.data/searchresult); null jika pencarian tidak didukung.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Mengekstrak sorotan dari dokumen.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Contoh berikut menunjukkan cara mengekstrak sorotan yang berisi 3 kata:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a highlight:
     HighlightItem hl = parser.getHighlight(2, true, new HighlightOptions(10, 3));
     // Check if highlight extraction is supported
     if (hl == null) {
         System.out.println("Highlight extraction isn't supported");
         return;
     }
     // Print an extracted highlight
     System.out.println(String.format("At %d: %s", hl.getPosition(), hl.getText()));
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | posisi | int | Posisi awal sorotan. |
|
|  | isDirect | boolean | Nilai yang menunjukkan apakah ekstraksi sorotan bersifat langsung.  true  jika sorotan diekstrak dari posisi kanan; jika tidak,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi ekstraksi sorotan. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Mengekstrak daftar isi dari dokumen.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Contoh berikut menunjukkan cara mengekstrak daftar isi dari file EPUB:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleEpub)) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     // Check if toc extraction is supported
     if (!parser.getFeatures().isToc()) {
         System.out.println("Toc extraction isn't supported.");
         return;
     }
     // Get table of contents
     Iterable toc = parser.getToc();
     // Iterate over items
     for (TocItem i : toc) {
         // Print the Toc text
         System.out.println(i.getText());
         // Check if page index has a value
         if (i.getPageIndex() == null) {
             continue;
         }
         // Extract a page text
         try (TextReader reader = parser.getText(i.getPageIndex())) {
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - Sekumpulan item daftar isi;  null  jika ekstraksi daftar isi tidak didukung.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Mengekstrak metadata dari dokumen.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Contoh berikut menunjukkan cara mengekstrak metadata dari dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Extract metadata from the document
     Iterable metadata = parser.getMetadata();
     // Check if metadata extraction is supported
     if (metadata == null) {
         System.out.println("Metatada extraction isn't supported");
     }
     // Iterate over metadata items
     for (MetadataItem item : metadata) {
         // Print an item name and value
         System.out.println(String.format("%s: %s", item.getName(), item.getValue()));
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Sekumpulan item metadata;  null  jika ekstraksi metadata tidak didukung.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Mengekstrak anotasi dari dokumen.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Sekumpulan item anotasi;  null  jika ekstraksi anotasi tidak didukung.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Mengekstrak anotasi dari halaman dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Sekumpulan item anotasi;  null  jika ekstraksi anotasi tidak didukung.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Mengekstrak objek kontainer dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Contoh berikut menunjukkan cara mengekstrak teks dari entitas zip:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over zip entities
     for (ContainerItem item : attachments) {
         // Print the file path
         System.out.println(item.getFilePath());
         try {
             // Create Parser object for the zip entity content
             try (Parser attachmentParser = item.openParser()) {
                 // Extract an zip entity text
                 try (TextReader reader = attachmentParser.getText()) {
                     System.out.println(reader == null ? "No text" : reader.readToEnd());
                 }
             }
         } catch (UnsupportedDocumentFormatException ex) {
             System.out.println("Isn't supported.");
         }
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Sekumpulan item kontainer;  null  jika ekstraksi kontainer tidak didukung.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Mengekstrak area teks dari dokumen.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Contoh berikut menunjukkan cara mengekstrak semua area teks dari seluruh dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Extract text areas
     Iterable areas = parser.getTextAreas();
     // Check if text areas extraction is supported
     if (areas == null) {
         System.out.println("Page text areas extraction isn't supported");
         return;
     }
     // Iterate over page text areas
     for (PageTextArea a : areas) {
         // Print a page index, rectangle and text area value:
         System.out.println(String.format("Page: %d, R: %s, Text: %s", a.getPage().getIndex(), a.getRectangle(), a.getText()));
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Sekumpulan objek [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  jika ekstraksi area teks tidak didukung.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Mengekstrak area teks dari dokumen menggunakan opsi penyesuaian (ekspresi reguler, cocokkan huruf, dll).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Contoh berikut menunjukkan cara mengekstrak hanya area teks dengan digit dari sudut kiri atas:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Create the options which are used for text area extraction
     PageTextAreaOptions options = new PageTextAreaOptions("\\s[a-z]{2}\\s", new Rectangle(new Point(0, 0), new Size(300, 100)));
     // Extract text areas which contain only digits from the upper-left corner of a page:
     Iterable areas = parser.getTextAreas(options);
     // Check if text areas extraction is supported
     if (areas == null) {
         System.out.println("Page text areas extraction isn't supported");
         return;
     }
     // Iterate over page text areas
     for (PageTextArea a : areas) {
         // Print a page index, rectangle and text area value:
         System.out.println(String.format("Page: %d, R: %s, Text: %s", a.getPage().getIndex(), a.getRectangle(), a.getText()));
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Opsi untuk ekstraksi area teks. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Sekumpulan objek [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  jika ekstraksi area teks tidak didukung.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Mengekstrak area teks dari halaman dokumen.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Untuk mengekstrak area teks dari halaman dokumen, metode berikut digunakan:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Check if the document supports text areas extraction
     if (!parser.getFeatures().isTextAreas()) {
         System.out.println("Document isn't supports text areas extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Iterate over page text areas
         // We ignore null-checking as we have checked text areas extraction feature support earlier
         for (PageTextArea a : parser.getTextAreas(pageIndex)) {
             // Print a rectangle and text area value:
             System.out.println(String.format("R: %s, Text: %s", a.getRectangle(), a.getText()));
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Sekumpulan objek [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  jika ekstraksi area teks tidak didukung.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Mengekstrak area teks dari halaman dokumen menggunakan opsi penyesuaian (ekspresi reguler, cocokkan huruf, dll).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Opsi untuk ekstraksi area teks. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Sekumpulan objek [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  jika ekstraksi area teks tidak didukung.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Mengekstrak gambar dari dokumen.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Contoh berikut menunjukkan cara mengekstrak semua gambar dari seluruh dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Extract images
     Iterable images = parser.getImages();
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Images extraction isn't supported");
         return;
     }
     // Iterate over images
     for (PageImageArea image : images) {
         // Print a page index, rectangle and image type:
         System.out.println(String.format("Page: %d, R: %s, Type: %s", image.getPage().getIndex(), image.getRectangle(), image.getFileType()));
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Sekumpulan objek [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  jika ekstraksi gambar tidak didukung.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Mengekstrak gambar dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Contoh berikut menunjukkan cara mengekstrak hanya gambar dari sudut kiri atas:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Create the options which are used for images extraction
     PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(340, 150), new Size(300, 100)));
     // Extract images from the upper-left corner of a page:
     Iterable images = parser.getImages(options);
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }
     // Iterate over images
     for (PageImageArea image : images) {
         // Print a page index, rectangle and image type:
         System.out.println(String.format("Page: %d, R: %s, Type: %s", image.getPage().getIndex(), image.getRectangle(), image.getFileType()));
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Opsi untuk ekstraksi gambar. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Sekumpulan objek [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  jika ekstraksi gambar tidak didukung.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Mengekstrak gambar dari halaman dokumen.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Untuk mengekstrak gambar dari halaman dokumen, metode berikut digunakan:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Check if the document supports images extraction
     if (!parser.getFeatures().isImages()) {
         System.out.println("Document isn't supports images extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Iterate over images
         // We ignore null-checking as we have checked images extraction feature support earlier
         for (PageImageArea image : parser.getImages(pageIndex)) {
             // Print a rectangle and image type
             System.out.println(String.format("R: %s, Text: %s", image.getRectangle(), image.getFileType()));
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Sekumpulan objek [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  jika ekstraksi gambar tidak didukung.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Mengekstrak gambar dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Opsi untuk ekstraksi gambar. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Sekumpulan objek [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  jika ekstraksi gambar tidak didukung.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Mengekstrak tautan dari dokumen.

Contoh berikut menunjukkan cara mengekstrak semua hyperlink dari seluruh dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Extract hyperlinks from the document
     Iterable hyperlinks = parser.getHyperlinks();
     // Iterate over hyperlinks
     for (PageHyperlinkArea h : hyperlinks) {
         // Print the hyperlink text
         System.out.println(h.getText());
         // Print the hyperlink URL
         System.out.println(h.getUrl());
         System.out.println();
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Sekumpulan objek [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  jika ekstraksi hyperlink tidak didukung.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Mengekstrak tautan dari halaman dokumen.

Contoh berikut menunjukkan cara mengekstrak hyperlink dari halaman dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Extract hyperlinks from the document page
         Iterable hyperlinks = parser.getHyperlinks(pageIndex);
         // Iterate over hyperlinks
         for (PageHyperlinkArea h : hyperlinks) {
             // Print the hyperlink text
             System.out.println(h.getText());
             // Print the hyperlink URL
             System.out.println(h.getUrl());
             System.out.println();
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Sekumpulan objek [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  jika ekstraksi hyperlink tidak didukung.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Mengekstrak tautan dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan).

Contoh berikut menunjukkan cara mengekstrak hyperlink dari area halaman dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.HyperlinksPdf)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Create the options which are used for hyperlink extraction
     PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
     // Extract hyperlinks from the document page area
     Iterable hyperlinks = parser.getHyperlinks(options);
     // Iterate over hyperlinks
     for (PageHyperlinkArea h : hyperlinks) {
         // Print the hyperlink text
         System.out.println(h.getText());
         // Print the hyperlink URL
         System.out.println(h.getUrl());
         System.out.println();
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Opsi untuk ekstraksi hyperlink. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Sekumpulan objek [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  jika ekstraksi hyperlink tidak didukung.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Mengekstrak tautan dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan).

Contoh berikut menunjukkan cara mengekstrak hyperlink dari area halaman dokumen menggunakan opsi penyesuaian:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Create the options which are used for hyperlink extraction
     PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Extract hyperlinks from the document page
         Iterable hyperlinks = parser.getHyperlinks(pageIndex, options);
         // Iterate over hyperlinks
         for (PageHyperlinkArea h : hyperlinks) {
             // Print the hyperlink text
             System.out.println(h.getText());
             // Print the hyperlink URL
             System.out.println(h.getUrl());
             System.out.println();
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Opsi untuk ekstraksi hyperlink. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Sekumpulan objek [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  jika ekstraksi hyperlink tidak didukung.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Mengekstrak kode batang dari dokumen.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Sekumpulan objek [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  jika ekstraksi barcode tidak didukung.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Mengekstrak kode batang dari halaman dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Sekumpulan objek [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  jika ekstraksi barcode tidak didukung.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Mengekstrak kode batang dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi kode batang).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Opsi untuk ekstraksi barcode. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Sekumpulan objek [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  jika ekstraksi barcode tidak didukung.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Mengekstrak kode batang dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi kode batang).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Opsi untuk ekstraksi barcode. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Sekumpulan objek [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  jika ekstraksi barcode tidak didukung.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Mengekstrak tabel dari dokumen.

Contoh berikut menunjukkan cara mengekstrak tabel dari seluruh dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports table extraction
     if (!parser.getFeatures().isTables()) {
         System.out.println("Document isn't supports tables extraction.");
         return;
     }
     // Create the layout of tables
     TemplateTableLayout layout = new TemplateTableLayout(
             java.util.Arrays.asList(new Double[]{50.0, 95.0, 275.0, 415.0, 485.0, 545.0}),
             java.util.Arrays.asList(new Double[]{325.0, 340.0, 365.0, 395.0}));
     // Create the options for table extraction
     PageTableAreaOptions options = new PageTableAreaOptions(layout);
     // Extract tables from the document
     Iterable tables = parser.getTables(options);
     // Iterate over tables
     for (PageTableArea t : tables) {
         // Iterate over rows
         for (int row = 0; row < t.getRowCount(); row++) {
             // Iterate over columns
             for (int column = 0; column < t.getColumnCount(); column++) {
                 // Get the table cell
                 PageTableAreaCell cell = t.getCell(row, column);
                 if (cell != null) {
                     // Print the table cell text
                     System.out.print(cell.getText());
                     System.out.print(" | ");
                 }
             }
             System.out.println();
         }
         System.out.println();
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Opsi untuk ekstraksi tabel. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Sekumpulan objek [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  jika ekstraksi tabel tidak didukung.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Mengekstrak tabel dari dokumen, mendeteksinya secara otomatis.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Sekumpulan objek [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  jika ekstraksi tabel tidak didukung.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Mengekstrak tabel dari halaman dokumen.

Contoh berikut menunjukkan cara mengekstrak tabel dari halaman dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleInvoicePagesPdf)) {
     // Check if the document supports table extraction
     if (!parser.getFeatures().isTables()) {
         System.out.println("Document isn't supports tables extraction.");
         return;
     }
     // Create the layout of tables
     TemplateTableLayout layout = new TemplateTableLayout(
             java.util.Arrays.asList(new Double[]{50.0, 95.0, 275.0, 415.0, 485.0, 545.0}),
             java.util.Arrays.asList(new Double[]{325.0, 340.0, 365.0, 395.0}));
     // Create the options for table extraction
     PageTableAreaOptions options = new PageTableAreaOptions(layout);
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Extract tables from the document page
         Iterable tables = parser.getTables(pageIndex, options);
         // Iterate over tables
         for (PageTableArea t : tables) {
             // Iterate over rows
             for (int row = 0; row < t.getRowCount(); row++) {
                 // Iterate over columns
                 for (int column = 0; column < t.getColumnCount(); column++) {
                     // Get the table cell
                     PageTableAreaCell cell = t.getCell(row, column);
                     if (cell != null) {
                         // Print the table cell text
                         System.out.print(cell.getText());
                         System.out.print(" | ");
                     }
                 }
                 System.out.println();
             }
             System.out.println();
         }
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Opsi untuk ekstraksi tabel. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Sekumpulan objek [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  jika ekstraksi tabel tidak didukung.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Mengekstrak tabel dari halaman dokumen, mendeteksinya secara otomatis.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Sekumpulan objek [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  jika ekstraksi tabel tidak didukung.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Menghasilkan kumpulan penyesuaian [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s untuk dokumen.

Cermin Java dari C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (commit d4e691b /
ae9e98c). Berguna sebagai templat awal yang kemudian dapat dipangkas atau diganti nama oleh pengguna.

### Algorithm

1. Pilih halaman dari  options.getPageIndex()  (default  0 ).
2. Jika dokumen mendukung ekstraksi area teks, panggil #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) dan hasilkan satu [TemplateField](../../com.groupdocs.parser.templates/templatefield) per area teks yang tidak kosong, dengan nama  {prefix}_{n}  (prefiks default  \"Field\" ). Setiap bidang mendapatkan [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) pada persegi panjang area teks, dengan lebar halaman dicatat sebagai  pageWidth  sehingga penskalaan templat berikutnya berfungsi.
3. Jika dokumen tidak mendukung area teks, kembalikan  null .

### OCR caveat

Implementasi C# menjalankan OCR pada pratinjau halaman untuk menghasilkan bidang ketika dokumen hanya berupa gambar. [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) milik Java disediakan pengguna, sehingga generasi berbasis OCR hanya bermakna jika sebuah konektor dikonfigurasi DAN fungsi  recognizeTextAreas(...)  pada konektor mengembalikan persegi panjang yang tepat. Ketika  options.getOcrOptions()  diatur dan sebuah konektor tersedia, pipeline OCR lebih dipilih.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Opsi generasi. Bisa jadi  null  (nilai baku diterapkan). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Iterable dari [TemplateItem](../../com.groupdocs.parser.templates/templateitem) yang dihasilkan, atau  null  jika tidak didukung oleh format dokumen ini.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Mengekstrak info tentang semua lembar kerja dalam spreadsheet.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Daftar instance [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) yang berisi informasi tentang semua lembar kerja dalam spreadsheet.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Mengekstrak info tentang lembar kerja.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | worksheetIndex | int | Indeks berbasis nol dari lembar kerja. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Mengekstrak sel lembar kerja.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | worksheetIndex | int | Indeks berbasis nol dari lembar kerja. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Sekumpulan instance [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) yang berisi data sel.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Mengekstrak sel lembar kerja menggunakan opsi penyesuaian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | worksheetIndex | int | Indeks berbasis nol dari lembar kerja. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Opsi ekstraksi lembar kerja. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Sekumpulan instance [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) yang berisi data sel.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Menganalisis dokumen dengan templat yang dibuat pengguna.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Templat yang dibuat pengguna. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Menganalisis dokumen dengan templat yang dibuat pengguna menggunakan opsi yang disediakan.

Jika
options.getPageIndex()
diatur, hanya halaman itu yang diproses; jika tidak, semua halaman diproses.

Dukungan OCR tergantung pada [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) yang dikonfigurasi dalam [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Templat yang dibuat pengguna. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Opsi parse-by-template. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Menganalisis dokumen dengan secara otomatis memilih templat yang paling cocok dari koleksi.

Cermin dari C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
diperkenalkan dalam commit 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), dan template yang menghasilkan
jumlah tertinggi bidang yang terisi (area halaman non-null dengan teks tidak kosong) menang. Implementasi C# menggunakan
pencocokan hidden-marker terhadap proses OCR; jalur itu belum tersedia di Java karena penanda hidden-field dan
TemplatePageOcrParser yang digerakkan OCR belum dipindahkan, sehingga hitungan bidang terisi ini digunakan sebagai fallback transparan.
Pemanggil yang memerlukan perilaku identik dengan C# harus memasang selector khusus setelah mesin OCR terhubung.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Koleksi templat kandidat. Parser akan memilih yang paling cocok. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Opsi parse. Mungkin null. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Menganalisis formulir dokumen.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Contoh berikut menunjukkan cara memproses sebuah formulir dokumen:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### getStructure() {#getStructure--}
```
public Document getStructure()
```


Mengekstrak teks terstruktur dari dokumen.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - Sebuah instance dari kelas org.w3c.dom.Document dengan struktur teks XML; null jika ekstraksi struktur teks tidak didukung.

### close() {#close--}
```
public void close()
```


Menutup sumber daya ini, melepaskan semua sumber daya yang mendasarinya.


