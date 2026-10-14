---
title: "EmailImapConnection"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi koneksi email untuk protokol IMAP."
type: docs
weight: 14
url: /id/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Mewakili informasi koneksi email untuk protokol IMAP.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getHost()](#getHost--) | Mendapatkan nama host. |
|
|  | [getPort()](#getPort--) | Mendapatkan nomor port. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Menginisialisasi instance baru dari kelas [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | host | java.lang.String | Nama host. |
|
|  | port | int | Nomor port. |
|
|  | userName | java.lang.String | Nama pengguna. |
|
|  | kata sandi | java.lang.String | Kata sandi. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Mendapatkan nama host.


**Returns:**
java.lang.String - Nilai string yang mewakili nama host.

### getPort() {#getPort--}
```
public int getPort()
```


Mendapatkan nomor port.


**Returns:**
int - Nilai integer yang mewakili nomor port.

