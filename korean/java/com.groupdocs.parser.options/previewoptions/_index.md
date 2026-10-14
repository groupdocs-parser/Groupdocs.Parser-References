---
title: "PreviewOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다."
type: docs
weight: 34
url: /ko/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 클래스를 새 인스턴스로 초기화하여 출력 스트림이 닫히게 합니다. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 클래스를 새 인스턴스로 초기화하여 출력 스트림이 클라이언트에 반환되어 추가로 사용할 수 있게 합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 페이지 미리보기 너비를 가져옵니다. |
|
|  | [setWidth(int width)](#setWidth-int-) | 페이지 미리보기 너비를 설정합니다. |
|
|  | [getHeight()](#getHeight--) | 페이지 미리보기 높이를 가져옵니다. |
|
|  | [setHeight(int height)](#setHeight-int-) | 페이지 미리보기 높이를 설정합니다. |
|
|  | [getDpi()](#getDpi--) | dpi를 가져옵니다. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | dpi를 설정합니다. |
|
|  | [getPageNumbers()](#getPageNumbers--) | 미리보기를 생성할 페이지 번호 배열을 가져옵니다. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | 미리보기를 생성할 페이지 번호 배열을 설정합니다. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | 미리보기 이미지 형식을 가져옵니다. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | 미리보기 이미지 형식을 설정합니다. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | 페이지 스트림 생성 대리자의 인스턴스를 가져옵니다. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | 페이지 스트림 생성 대리자의 인스턴스를 설정합니다. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | 페이지 미리보기 완료 대리자의 인스턴스를 가져옵니다. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | 페이지 미리보기 완료 대리자의 인스턴스를 설정합니다. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | 페이지 미리보기 렌더 정보 대리자의 인스턴스를 가져옵니다. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | 페이지 미리보기 렌더 정보 대리자의 인스턴스를 설정합니다. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


[PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 클래스를 새 인스턴스로 초기화하여 출력 스트림이 닫히게 합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 특정 페이지 미리보기를 위한 스트림을 생성합니다. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


[PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 클래스를 새 인스턴스로 초기화하여 출력 스트림이 클라이언트에 반환되어 추가로 사용할 수 있게 합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 특정 페이지 미리보기를 위한 스트림을 생성합니다 |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | 페이지 미리보기 생성이 완료되었음을 알리고 출력 스트림을 가져옵니다. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


페이지 미리보기 너비를 가져옵니다.


**Returns:**
int - 페이지 너비.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


페이지 미리보기 너비를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 너비 | int | 페이지 너비. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


페이지 미리보기 높이를 가져옵니다.


**Returns:**
int - 페이지 높이.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


페이지 미리보기 높이를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 높이 | int | 페이지 높이. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


dpi를 가져옵니다.


**Returns:**
int - dpi를 나타내는 정수 값.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


dpi를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | dpi | int | DPI. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


미리보기를 생성할 페이지 번호 배열을 가져옵니다.


**Returns:**
int[] - 페이지 번호의 컬렉션.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


미리보기를 생성할 페이지 번호 배열을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageNumbers | int[] | 페이지 번호의 컬렉션. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


미리보기 이미지 형식을 가져옵니다.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


미리보기 이미지 형식을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | 미리보기 형식. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


페이지 스트림 생성 대리자의 인스턴스를 가져옵니다.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


페이지 스트림 생성 대리자의 인스턴스를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 페이지 스트림 생성 위임자. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


페이지 미리보기 완료 대리자의 인스턴스를 가져옵니다.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


페이지 미리보기 완료 대리자의 인스턴스를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | 페이지 미리보기 완료 위임자. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


페이지 미리보기 렌더 정보 대리자의 인스턴스를 가져옵니다.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


페이지 미리보기 렌더 정보 대리자의 인스턴스를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | 페이지 미리보기 렌더링 정보 위임자. |
|

