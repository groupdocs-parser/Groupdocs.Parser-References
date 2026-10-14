---
title: "QualityMode"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "品質のレベルを定義します。"
type: docs
weight: 48
url: /ja/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

品質のレベルを定義します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [High](#High) | 高品質。 |
|
|  | [Normal](#Normal) | 標準品質。 |
|
|  | [Low](#Low) | 低品質。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


高品質。高速な処理アルゴリズムが使用されます。


### Normal {#Normal}
```
public static final QualityMode Normal
```


標準品質。デフォルトの処理アルゴリズムが使用されます。


### Low {#Low}
```
public static final QualityMode Low
```


低品質。低速な処理アルゴリズムが使用されます。


### values() {#values--}
```
public static QualityMode[] values()
```




**Returns:**
com.groupdocs.parser.options.QualityMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static QualityMode valueOf(String name)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
