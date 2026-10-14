---
title: "MetadataItem"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "컨테이너 항목 및 메타데이터 추출 기능에서 사용되는 메타데이터 항목을 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

컨테이너 항목 및 메타데이터 추출 기능에서 사용되는 메타데이터 항목을 나타냅니다.

[MetadataItem](../../com.groupdocs.parser.data/metadataitem) 클래스의 인스턴스는 [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) 메서드의 반환값으로 사용됩니다.
그리고 [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) 컬렉션의 항목으로도 사용됩니다. 사용 예제를 확인하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | [MetadataItem](../../com.groupdocs.parser.data/metadataitem) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getName()](#getName--) | 메타데이터 항목의 이름을 가져옵니다. |
|
|  | [getValue()](#getValue--) | 메타데이터 항목의 값을 가져옵니다. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


[MetadataItem](../../com.groupdocs.parser.data/metadataitem) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 이름 | java.lang.String | 메타데이터 항목의 이름. |
|
|  | 값 | java.lang.String | 메타데이터 항목의 값. |
|

### getName() {#getName--}
```
public String getName()
```


메타데이터 항목의 이름을 가져옵니다.


**Returns:**
java.lang.String - 메타데이터 항목의 이름을 나타내는 문자열 값.

### getValue() {#getValue--}
```
public String getValue()
```


메타데이터 항목의 값을 가져옵니다.


**Returns:**
java.lang.String - 메타데이터 항목의 값을 나타내는 문자열 값.

