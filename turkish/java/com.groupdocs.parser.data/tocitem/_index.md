---
title: "TocItem"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "İçindekiler tablosu çıkarma işlevselliğinde kullanılan öğeyi temsil eder."
type: docs
weight: 31
url: /tr/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

İçindekiler tablosu çıkarma işlevselliğinde kullanılan öğeyi temsil eder.

Bir [TocItem](../../com.groupdocs.parser.data/tocitem) sınıfı örneği, [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) metodunun dönüş değeri olarak kullanılır. Oradaki kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | TocItem sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDepth()](#getDepth--) | Derinlik seviyesini alır. |
|
|  | [getText()](#getText--) | Metni alır. |
|
|  | [getPageIndex()](#getPageIndex--) | Sayfa indeksini alır. |
|
|  | [extractText()](#extractText--) | TocItem nesnesinin işaret ettiği belgeden bir metin çıkarır. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


TocItem sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | depth | int | Öğenin derinlik seviyesi. |
|
|  | metin | java.lang.String | Öğenin metni. |
|
|  | pageIndex | java.lang.Integer | Öğe tarafından referans verilen sayfanın indeksi |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Derinlik seviyesini alır.


**Returns:**
int - Öğenin derinlik seviyesini temsil eden bir tam sayı değeri.

### getText() {#getText--}
```
public String getText()
```


Metni alır.


**Returns:**
java.lang.String - Öğenin metnini temsil eden bir dize değeri.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Sayfa indeksini alır.


**Returns:**
java.lang.Integer - Öğenin referans verdiği sayfanın indeksini temsil eden bir tam sayı değeri;  null  ayarlanmamışsa.

### extractText() {#extractText--}
```
public TextReader extractText()
```


TocItem nesnesinin işaret ettiği belgeden bir metin çıkarır.

Aşağıdaki örnek, içindekiler tablosundaki bir öğe ile metin nasıl çıkarılacağını gösterir:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

