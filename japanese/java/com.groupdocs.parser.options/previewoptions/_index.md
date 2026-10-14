---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。"
type: docs
weight: 34
url: /ja/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | 新しい [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) クラスのインスタンスを初期化し、出力ストリームを閉じます。 |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | 新しい [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) クラスのインスタンスを初期化し、出力ストリームをクライアントに返してさらに使用できるようにします。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getWidth()](#getWidth--) | ページプレビューの幅を取得します。 |
|
|  | [setWidth(int width)](#setWidth-int-) | ページプレビューの幅を設定します。 |
|
|  | [getHeight()](#getHeight--) | ページプレビューの高さを取得します。 |
|
|  | [setHeight(int height)](#setHeight-int-) | ページプレビューの高さを設定します。 |
|
|  | [getDpi()](#getDpi--) | dpi を取得します。 |
|
|  | [setDpi(int dpi)](#setDpi-int-) | dpi を設定します。 |
|
|  | [getPageNumbers()](#getPageNumbers--) | プレビューを生成するページ番号の配列を取得します。 |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | プレビューを生成するページ番号の配列を設定します。 |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | プレビュー画像のフォーマットを取得します。 |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | プレビュー画像のフォーマットを設定します。 |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | ページストリーム作成デリゲートのインスタンスを取得します。 |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | ページストリーム作成デリゲートのインスタンスを設定します。 |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | ページプレビュー完了デリゲートのインスタンスを取得します。 |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | ページプレビュー完了デリゲートのインスタンスを設定します。 |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | ページプレビュー描画情報デリゲートのインスタンスを取得します。 |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | ページプレビュー描画情報デリゲートのインスタンスを設定します。 |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


新しい [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) クラスのインスタンスを初期化し、出力ストリームを閉じます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 特定のページプレビュー用のストリームを作成します。 |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


新しい [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) クラスのインスタンスを初期化し、出力ストリームをクライアントに返してさらに使用できるようにします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 特定のページプレビュー用のストリームを作成します |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | ページプレビューの生成が完了したことを通知し、出力ストリームを取得します。 |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


ページプレビューの幅を取得します。


**Returns:**
int - ページ幅。

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


ページプレビューの幅を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | width | int | ページ幅。 |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


ページプレビューの高さを取得します。


**Returns:**
int - ページ高さ。

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


ページプレビューの高さを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | height | int | ページ高さ。 |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


dpi を取得します。


**Returns:**
int - dpi を表す整数値。

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


dpi を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | dpi | int | dpi。 |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


プレビューを生成するページ番号の配列を取得します。


**Returns:**
int[] - ページ番号のコレクション。

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


プレビューを生成するページ番号の配列を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageNumbers | int[] | ページ番号のコレクション。 |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


プレビュー画像のフォーマットを取得します。


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


プレビュー画像のフォーマットを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | プレビュー形式。 |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


ページストリーム作成デリゲートのインスタンスを取得します。


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


ページストリーム作成デリゲートのインスタンスを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | ページストリーム作成デリゲート。 |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


ページプレビュー完了デリゲートのインスタンスを取得します。


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


ページプレビュー完了デリゲートのインスタンスを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | ページプレビュー完了デリゲート。 |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


ページプレビュー描画情報デリゲートのインスタンスを取得します。


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


ページプレビュー描画情報デリゲートのインスタンスを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | ページプレビュー描画情報デリゲート。 |
|

