---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "バーコード抽出に使用されるオプションを提供します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

バーコード抽出に使用されるオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | BarcodeOptions クラスの新しいインスタンスをデフォルト値で初期化します。 |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | BarcodeOptions クラスの新しいインスタンスを矩形領域で初期化します。 |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | BarcodeOptions クラスの新しいインスタンスを品質設定とコードタイプで初期化します。 |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | BarcodeOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | 不正なバーコードが許可されているかどうかを示す値を取得します。 |
|
|  | [getDimension()](#getDimension--) | バーコードの最小要素の最小サイズを取得します。 |
|
|  | [getImageQuality()](#getImageQuality--) | ソース画像の品質を取得します。 |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | ソースバーコードの品質を取得します。 |
|
|  | [getRectangle()](#getRectangle--) | ページ領域を含む矩形領域を取得します。 |
|
|  | [getCodeTypes()](#getCodeTypes--) | 読み取るバーコードのタイプを取得します。 |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | 不正なバーコードが許可されているかどうかを示す値を設定します。 |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | バーコードの最小要素の最小サイズを設定します。 |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | ソース画像の品質を設定します。 |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | ソースバーコードの品質を設定します。 |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | バーコードを含む矩形領域を設定します。 |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | 読み取るバーコードのタイプを設定します。 |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


BarcodeOptions クラスの新しいインスタンスをデフォルト値で初期化します。


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


BarcodeOptions クラスの新しいインスタンスを矩形領域で初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | バーコードを含む矩形領域です。 |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


BarcodeOptions クラスの新しいインスタンスを品質設定とコードタイプで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | ソース画像の品質です。 |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | ソースバーコードの品質です。 |
|
|  | codeTypes | java.lang.String[] | 読み取るバーコードの種類。 |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


BarcodeOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | バーコードを含む矩形領域です。 |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | ソース画像の品質です。 |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | ソースバーコードの品質です。 |
|
|  | dimension | java.lang.Float | バーコードの最小要素の最小サイズ。 |
|
|  | allowIncorrectBarcodes | boolean | 不正なバーコードが許可されているかどうかを示す値。 |
|
|  | codeTypes | java.lang.String[] | 読み取るバーコードの種類。 |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


不正なバーコードが許可されているかどうかを示す値を取得します。


**Returns:**
boolean - 不正なバーコードが許可されている場合は true、そうでない場合は false。

### getDimension() {#getDimension--}
```
public Float getDimension()
```


バーコードの最小要素の最小サイズを取得します。


**Returns:**
java.lang.Float - バーコードの最小要素を表す浮動小数点値。自動モードが使用される場合は null。

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


ソース画像の品質を取得します。


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


ソースバーコードの品質を取得します。


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


ページ領域を含む矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


読み取るバーコードのタイプを取得します。


**Returns:**
java.util.List<java.lang.String> - 読み取るバーコードの種類を含む読み取り専用コレクション。設定されていない場合は空のコレクション。

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


不正なバーコードが許可されているかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | 不正なバーコードが許可されている場合は true。 |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


バーコードの最小要素の最小サイズを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | dimension | java.lang.Float | バーコードの最小要素。自動モードの場合は null。 |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


ソース画像の品質を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 画像品質モード。 |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


ソースバーコードの品質を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | バーコード品質モード。 |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


バーコードを含む矩形領域を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 矩形領域。ページ全体をスキャンする場合は null。 |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


読み取るバーコードのタイプを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | バーコードの種類。すべての種類の場合は null または空。 |
|

