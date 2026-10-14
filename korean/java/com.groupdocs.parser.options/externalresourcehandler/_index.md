---
title: "ExternalResourceHandler"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "외부 리소스 로드를 위한 핸들러를 제공합니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

외부 리소스 로드를 위한 핸들러를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | 외부 리소스를 로드하기 전에 호출됩니다. |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


외부 리소스를 로드하기 전에 호출됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | 외부 리소스 로드를 제어하기 위한 데이터. |
|

