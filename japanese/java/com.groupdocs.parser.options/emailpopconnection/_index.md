---
title: "EmailPopConnection"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "POP プロトコル用のメール接続情報を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

POP プロトコル用のメール接続情報を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | 新しい [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getHost()](#getHost--) | ホスト名を取得します。 |
|
|  | [getPort()](#getPort--) | ポート番号を取得します。 |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


新しい [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | host | java.lang.String | ホスト名です。 |
|
|  | port | int | ポート番号です。 |
|
|  | userName | java.lang.String | ユーザー名です。 |
|
|  | password | java.lang.String | パスワードです。 |
|

### getHost() {#getHost--}
```
public String getHost()
```


ホスト名を取得します。


**Returns:**
java.lang.String - ホスト名を表す文字列値です。

### getPort() {#getPort--}
```
public int getPort()
```


ポート番号を取得します。


**Returns:**
int - ポート番号を表す整数値です。

