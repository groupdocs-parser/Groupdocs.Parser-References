---
title: "ExternalResourceHandler"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "外部リソースの読み込み用ハンドラを提供します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

外部リソースの読み込み用ハンドラを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | 外部リソースがロードされる前に呼び出されます。 |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


外部リソースがロードされる前に呼び出されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | 外部リソースの読み込みを制御するためのデータです。 |
|

