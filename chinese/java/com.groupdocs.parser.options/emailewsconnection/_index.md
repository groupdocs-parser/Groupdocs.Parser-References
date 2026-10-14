---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于 EWS 协议的电子邮件连接信息。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

表示用于 EWS 协议的电子邮件连接信息。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | 初始化 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 类的新实例。 |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 初始化 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | 获取邮箱的 URI。 |
|
|  | [getDomain()](#getDomain--) | 获取域名。 |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


初始化 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | 邮箱的 URI。 |
|
|  | userName | java.lang.String | 用户名。 |
|
|  | 密码 | java.lang.String | 密码。 |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


初始化 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | 邮箱的 URI。 |
|
|  | domain | java.lang.String | 域名。 |
|
|  | userName | java.lang.String | 用户名。 |
|
|  | 密码 | java.lang.String | 密码。 |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


获取邮箱的 URI。


**Returns:**
java.lang.String - 一个表示邮箱 URI 的字符串值。

### getDomain() {#getDomain--}
```
public String getDomain()
```


获取域名。


**Returns:**
java.lang.String - 一个表示域名的字符串值。

