---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "IMAP プロトコル用のメール接続情報を表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

IMAP プロトコル用のメール接続情報を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getHost()](#getHost--) | ホスト名を取得します。 |
|
|  | [getPort()](#getPort--) | ポート番号を取得します。 |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


[EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) クラスの新しいインスタンスを初期化します。


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

