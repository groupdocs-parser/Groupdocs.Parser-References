---
title: "TemplateOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート機能による解析に使用されるオプションを提供します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

テンプレート機能による解析に使用されるオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | 新しい [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | 矩形領域でキャプチャされる際に無視される境界のサイズを取得します。 |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


新しい [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangleTolerance | double | 矩形領域でキャプチャされる際に無視される境界のサイズです。テキスト項目の高さの割合で測定されます。 |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


矩形領域でキャプチャされる際に無視される境界のサイズを取得します。テキスト項目の高さの割合で測定されます。


**Returns:**
double - 0（境界なし）から 1（要素全体を無視）までの double 値です。

