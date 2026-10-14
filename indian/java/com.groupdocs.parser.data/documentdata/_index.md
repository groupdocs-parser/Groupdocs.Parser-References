---
title: "DocumentData"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "दस्तावेज़ का डेटा दर्शाता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

दस्तावेज़ का डेटा दर्शाता है। यह [FieldData](../../com.groupdocs.parser.data/fielddata) ऑब्जेक्ट्स से बना है जो दस्तावेज़ से फ़ील्ड डेटा रखते हैं। [DocumentData](../../com.groupdocs.parser.data/documentdata) क्लास का एक इंस्टेंस [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) और [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) मेथड्स के रिटर्न वैल्यू के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | इस दस्तावेज़ डेटा को उत्पन्न करने वाले टेम्प्लेट को प्राप्त करता है। |
|
|  | [getCount()](#getCount--) | फ़ील्ड डेटा की कुल संख्या प्राप्त करता है। |
|
|  | [get(int index)](#get-int-) | इंडेक्स द्वारा फ़ील्ड डेटा प्राप्त करता है। |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | फ़ील्ड डेटा का संग्रह लौटाता है जहाँ नाम  fieldName  के बराबर हो। |
|
|  | [iterator()](#iterator--) | इस सूची में तत्वों पर उचित क्रम में एक इटररेटर लौटाता है। |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


इस दस्तावेज़ डेटा को उत्पन्न करने वाले टेम्प्लेट को प्राप्त करता है।

जब डेटा स्वचालित टेम्पलेट-संग्रह चयन द्वारा उत्पन्न किया गया था (देखें
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
यह चयनित टेम्पलेट है।
null
जब डेटा टेम्पलेट द्वारा उत्पन्न नहीं किया गया था।


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


फ़ील्ड डेटा की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो फ़ील्ड डेटा की कुल संख्या का प्रतिनिधित्व करता है।

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


इंडेक्स द्वारा फ़ील्ड डेटा प्राप्त करता है।

सभी फ़ील्ड्स के माध्यम से पुनरावृत्ति:

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
[PageArea](../../com.groupdocs.parser.data/pagearea) क्लास के उत्तराधिकारियों का। उदाहरण के लिए, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) मेथड केवल टेक्स्ट फ़ील्ड्स निकालता है:

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



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | फ़ील्ड का शून्य-आधारित अनुक्रमणिका। |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


फ़ील्ड डेटा का संग्रह लौटाता है जहाँ नाम  fieldName  के बराबर हो।

फ़ील्ड नाम द्वारा फ़ील्ड्स खोजें:

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
[PageArea](../../com.groupdocs.parser.data/pagearea) क्लास के किसी भी उत्तराधिकारियों का। उदाहरण के लिए, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) मेथड केवल टेक्स्ट फ़ील्ड्स निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fieldName | java.lang.String | फ़ील्ड का नाम। |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - [FieldData](../../com.groupdocs.parser.data/fielddata) ऑब्जेक्ट्स का संग्रह; यदि कोई फ़ील्ड डेटा नहीं मिला तो खाली संग्रह।

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


इस सूची में तत्वों पर उचित क्रम में एक इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - इस सूची में तत्वों पर उचित क्रम में इटररेटर।

