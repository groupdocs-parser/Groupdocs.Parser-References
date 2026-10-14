---
title: "라이선스"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "GroupDocs.Parser 라이선스를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

GroupDocs.Parser 라이선스를 나타냅니다.

이 예제는 라이선스를 설정하는 방법을 보여줍니다.

````
 ```

// Initialize License class
License license = new License();
// .lic 파일 경로 설정
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [License()](#License--) | 새 인스턴스를 초기화합니다 [License](../../com.groupdocs.parser.licensing/license) 클래스. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | 구성 요소에 라이선스를 적용합니다. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | 구성 요소에 라이선스를 적용합니다. |
|
### License() {#License--}
```
public License()
```


새 인스턴스를 초기화합니다 [License](../../com.groupdocs.parser.licensing/license) 클래스.


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


구성 요소에 라이선스를 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 라이선스 파일에 대한 절대 경로. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


구성 요소에 라이선스를 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 라이선스 스트림. |
|

