---
title: "BarcodeOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "바코드 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

바코드 추출에 사용되는 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | 기본값으로 BarcodeOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | 사각형 영역을 사용하여 BarcodeOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | 품질 설정 및 코드 유형과 함께 BarcodeOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | BarcodeOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | 잘못된 바코드가 허용되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getDimension()](#getDimension--) | 바코드 최소 요소의 최소 크기를 가져옵니다. |
|
|  | [getImageQuality()](#getImageQuality--) | 소스 이미지의 품질을 가져옵니다. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | 소스 바코드의 품질을 가져옵니다. |
|
|  | [getRectangle()](#getRectangle--) | 페이지 영역을 포함하는 사각형 영역을 가져옵니다. |
|
|  | [getCodeTypes()](#getCodeTypes--) | 읽을 바코드 유형을 가져옵니다. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | 잘못된 바코드가 허용되는지 여부를 나타내는 값을 설정합니다. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | 바코드 최소 요소의 최소 크기를 설정합니다. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | 소스 이미지의 품질을 설정합니다. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | 소스 바코드의 품질을 설정합니다. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | 바코드를 포함하는 직사각형 영역을 설정합니다. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | 읽을 바코드 유형을 설정합니다. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


기본값으로 BarcodeOptions 클래스의 새 인스턴스를 초기화합니다.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


사각형 영역을 사용하여 BarcodeOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 바코드를 포함하는 직사각형 영역. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


품질 설정 및 코드 유형과 함께 BarcodeOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 소스 이미지의 품질. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 소스 바코드의 품질. |
|
|  | codeTypes | java.lang.String[] | 읽을 바코드 유형. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


BarcodeOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 바코드를 포함하는 직사각형 영역. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 소스 이미지의 품질. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 소스 바코드의 품질. |
|
|  | dimension | java.lang.Float | 바코드 최소 요소의 최소 크기. |
|
|  | allowIncorrectBarcodes | boolean | 잘못된 바코드가 허용되는지 여부를 나타내는 값. |
|
|  | codeTypes | java.lang.String[] | 읽을 바코드 유형. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


잘못된 바코드가 허용되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  잘못된 바코드가 허용되는 경우; 그렇지 않으면  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


바코드 최소 요소의 최소 크기를 가져옵니다.


**Returns:**
java.lang.Float - 바코드 최소 요소를 나타내는 float 값; 자동 모드가 사용되는 경우  null  입니다.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


소스 이미지의 품질을 가져옵니다.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


소스 바코드의 품질을 가져옵니다.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


페이지 영역을 포함하는 사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


읽을 바코드 유형을 가져옵니다.


**Returns:**
java.util.List<java.lang.String> - 읽을 바코드 유형을 포함하는 읽기 전용 컬렉션; 설정되지 않은 경우 빈 컬렉션입니다.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


잘못된 바코드가 허용되는지 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | 잘못된 바코드가 허용되는 경우 true. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


바코드 최소 요소의 최소 크기를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | dimension | java.lang.Float | 바코드 최소 요소; 자동 모드의 경우  null . |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


소스 이미지의 품질을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 이미지 품질 모드. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


소스 바코드의 품질을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 바코드 품질 모드. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


바코드를 포함하는 직사각형 영역을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 사각형 영역; 전체 페이지를 스캔하려면  null . |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


읽을 바코드 유형을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | 바코드 유형; 모든 유형의 경우  null  또는 비어 있습니다. |
|

