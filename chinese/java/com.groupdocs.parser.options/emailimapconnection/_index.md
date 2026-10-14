---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于 IMAP 协议的电子邮件连接信息。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

表示用于 IMAP 协议的电子邮件连接信息。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | 初始化 [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getHost()](#getHost--) | 获取主机名。 |
|
|  | [getPort()](#getPort--) | 获取端口号。 |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


初始化 [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | host | java.lang.String | 主机名。 |
|
|  | port | int | 端口号。 |
|
|  | userName | java.lang.String | 用户名。 |
|
|  | 密码 | java.lang.String | 密码。 |
|

### getHost() {#getHost--}
```
public String getHost()
```


获取主机名。


**Returns:**
java.lang.String - 表示主机名的字符串值。

### getPort() {#getPort--}
```
public int getPort()
```


获取端口号。


**Returns:**
int - 表示端口号的整数值。

