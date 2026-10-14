---
title: "TocItem"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "목차 추출 기능에 사용되는 항목을 나타냅니다."
type: docs
weight: 31
url: /ko/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

목차 추출 기능에 사용되는 항목을 나타냅니다.

[TocItem](../../com.groupdocs.parser.data/tocitem) 클래스의 인스턴스는 [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) 메서드의 반환값으로 사용됩니다. 사용 예제는 해당 페이지를 참조하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | TocItem 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDepth()](#getDepth--) | 깊이 수준을 가져옵니다. |
|
|  | [getText()](#getText--) | 텍스트를 가져옵니다. |
|
|  | [getPageIndex()](#getPageIndex--) | 페이지 인덱스를 가져옵니다. |
|
|  | [extractText()](#extractText--) | TocItem 객체가 참조하는 문서에서 텍스트를 추출합니다. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


TocItem 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | depth | int | 항목의 깊이 수준. |
|
|  | 텍스트 | java.lang.String | 항목의 텍스트. |
|
|  | pageIndex | java.lang.Integer | 항목이 참조하는 페이지의 인덱스 |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


깊이 수준을 가져옵니다.


**Returns:**
int - 항목의 깊이 수준을 나타내는 정수 값.

### getText() {#getText--}
```
public String getText()
```


텍스트를 가져옵니다.


**Returns:**
java.lang.String - 항목의 텍스트를 나타내는 문자열 값.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


페이지 인덱스를 가져옵니다.


**Returns:**
java.lang.Integer - 항목이 참조하는 페이지의 인덱스를 나타내는 정수 값; 설정되지 않은 경우  null  입니다.

### extractText() {#extractText--}
```
public TextReader extractText()
```


TocItem 객체가 참조하는 문서에서 텍스트를 추출합니다.

다음 예제는 목차 항목을 사용하여 텍스트를 추출하는 방법을 보여줍니다:

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

