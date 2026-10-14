---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "EWS プロトコル用のメール接続情報を表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

EWS プロトコル用のメール接続情報を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | 新しい [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) クラスのインスタンスを初期化します。 |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 新しい [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | メールボックスの URI を取得します。 |
|
|  | [getDomain()](#getDomain--) | ドメイン名を取得します。 |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


新しい [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | メールボックスの URI です。 |
|
|  | userName | java.lang.String | ユーザー名です。 |
|
|  | password | java.lang.String | パスワードです。 |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


新しい [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | メールボックスの URI です。 |
|
|  | domain | java.lang.String | ドメイン名です。 |
|
|  | userName | java.lang.String | ユーザー名です。 |
|
|  | password | java.lang.String | パスワードです。 |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


メールボックスの URI を取得します。


**Returns:**
java.lang.String - メールボックスの URI を表す文字列値です。

### getDomain() {#getDomain--}
```
public String getDomain()
```


ドメイン名を取得します。


**Returns:**
java.lang.String - ドメイン名を表す文字列値です。

