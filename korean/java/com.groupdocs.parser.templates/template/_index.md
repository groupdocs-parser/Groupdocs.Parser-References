---
title: "Template"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "문서 페이지 템플릿을 제공합니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

문서 페이지 템플릿을 제공합니다. 템플릿 항목(예: 텍스트 필드 및 테이블 정의)을 나타내는 [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 객체들로 구성됩니다.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | 새로운 [Template](../../com.groupdocs.parser.templates/template) 클래스 인스턴스를 초기화합니다. |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | 새로운 [Template](../../com.groupdocs.parser.templates/template) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | 템플릿 항목의 총 개수를 가져옵니다. |
|
|  | [get(int index)](#get-int-) | 인덱스로 템플릿 항목을 가져옵니다. |
|
|  | [getOptions()](#getOptions--) | 템플릿 옵션을 가져옵니다. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | 파일에서 템플릿을 로드합니다. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | 스트림에서 템플릿을 로드합니다. |
|
|  | [save(String filePath)](#save-java.lang.String-) | 파일에 템플릿을 저장합니다. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | 스트림에 템플릿을 저장합니다. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


새로운 [Template](../../com.groupdocs.parser.templates/template) 클래스 인스턴스를 초기화합니다.

사용법:

````
// Create an array of template fields
 TemplateItem[] fields = new TemplateItem[]
 {
     new TemplateField(new TemplateRegexPosition("From"), "From", 0),
     new TemplateField(
         new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromCompany",
         0),
     new TemplateField(
         new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromAddress",
         0)
 };
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 객체들의 컬렉션입니다. |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


새로운 [Template](../../com.groupdocs.parser.templates/template) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 객체들의 컬렉션입니다. |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | 템플릿 옵션. |
|

### getCount() {#getCount--}
```
public int getCount()
```


템플릿 항목의 총 개수를 가져옵니다.


**Returns:**
int - 템플릿 항목의 총 개수를 나타내는 정수입니다.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


인덱스로 템플릿 항목을 가져옵니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 템플릿 항목의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


템플릿 옵션을 가져옵니다.


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


파일에서 템플릿을 로드합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


스트림에서 템플릿을 로드합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 입력 스트림입니다. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


파일에 템플릿을 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


스트림에 템플릿을 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | stream | java.io.OutputStream | 출력 스트림. |
|

