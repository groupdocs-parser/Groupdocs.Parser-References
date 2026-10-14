---
title: "DocumentData"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "문서 데이터를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

문서 데이터를 나타냅니다. 여기에는 문서에서 필드 데이터를 포함하는 [FieldData](../../com.groupdocs.parser.data/fielddata) 객체가 포함됩니다. [DocumentData](../../com.groupdocs.parser.data/documentdata) 클래스의 인스턴스는 [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) 및 [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 메서드의 반환 값으로 사용됩니다. 해당 사용 예제를 확인하십시오.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | 이 문서 데이터를 생성한 템플릿을 가져옵니다. |
|
|  | [getCount()](#getCount--) | 필드 데이터의 총 개수를 가져옵니다. |
|
|  | [get(int index)](#get-int-) | 인덱스로 필드 데이터를 가져옵니다. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | 이름이  fieldName  와 같은 필드 데이터 컬렉션을 반환합니다. |
|
|  | [iterator()](#iterator--) | 이 리스트의 요소들을 올바른 순서로 순회하는 반복자를 반환합니다. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


이 문서 데이터를 생성한 템플릿을 가져옵니다.

데이터가 자동 템플릿-컬렉션 선택에 의해 생성된 경우 (see
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
이것이 선택된 템플릿입니다.
null
데이터가 템플릿에 의해 생성되지 않은 경우.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


필드 데이터의 총 개수를 가져옵니다.


**Returns:**
int - 필드 데이터의 총 개수를 나타내는 정수 값입니다.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


인덱스로 필드 데이터를 가져옵니다.

모든 필드를 순회:

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
[PageArea](../../com.groupdocs.parser.data/pagearea) 클래스의 상속자들에 대해. 예를 들어, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 메서드는 텍스트 필드만 추출합니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 필드의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


이름이  fieldName  와 같은 필드 데이터 컬렉션을 반환합니다.

필드 이름으로 필드를 찾습니다:

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
[PageArea](../../com.groupdocs.parser.data/pagearea) 클래스의 모든 상속자. 예를 들어, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 메서드는 텍스트 필드만 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fieldName | java.lang.String | 필드의 이름입니다. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - [FieldData](../../com.groupdocs.parser.data/fielddata) 객체의 컬렉션이며, 필드 데이터가 없을 경우 빈 컬렉션입니다.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


이 리스트의 요소들을 올바른 순서로 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - 이 리스트의 요소들을 올바른 순서대로 순회하는 반복자입니다.

