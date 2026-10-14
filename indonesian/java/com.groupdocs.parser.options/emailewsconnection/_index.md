---
title: "EmailEwsConnection"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi koneksi email untuk protokol EWS."
type: docs
weight: 13
url: /id/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Mewakili informasi koneksi email untuk protokol EWS.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Mendapatkan URI kotak surat. |
|
|  | [getDomain()](#getDomain--) | Mendapatkan nama domain. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Menginisialisasi instance baru dari kelas [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI kotak surat. |
|
|  | userName | java.lang.String | Nama pengguna. |
|
|  | kata sandi | java.lang.String | Kata sandi. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Menginisialisasi instance baru dari kelas [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI kotak surat. |
|
|  | domain | java.lang.String | Nama domain. |
|
|  | userName | java.lang.String | Nama pengguna. |
|
|  | kata sandi | java.lang.String | Kata sandi. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Mendapatkan URI kotak surat.


**Returns:**
java.lang.String - Nilai string yang mewakili URI kotak surat.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Mendapatkan nama domain.


**Returns:**
java.lang.String - Nilai string yang mewakili nama domain.

