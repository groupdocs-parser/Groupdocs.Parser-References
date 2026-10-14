---
title: "DocumentPageData"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "문서 페이지 데이터를 나타냅니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

문서 페이지의 데이터를 나타냅니다. 여기에는 문서 페이지에서 필드 데이터를 포함하는 [FieldData](../../com.groupdocs.parser.data/fielddata) 객체가 포함됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | 페이지 인덱스를 가져옵니다. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


[DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 필드 | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | 필드 데이터 컬렉션. |
|
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


페이지 인덱스를 가져옵니다.


**Returns:**
int - 페이지의 0부터 시작하는 인덱스.

