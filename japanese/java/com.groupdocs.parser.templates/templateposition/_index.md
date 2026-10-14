---
title: "TemplatePosition"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート位置の基底抽象クラスを提供します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

テンプレート位置の基底抽象クラスを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | 現在の位置のコピーを作成し、すべての座標を指定された factor でスケーリングします。 |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


現在の位置のコピーを作成し、すべての座標を指定された factor でスケーリングします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | factor | double | スケーリング係数です。 |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

