---
title: "License"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "GroupDocs.Parser lisansını temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

GroupDocs.Parser lisansını temsil eder.

Bu örnek, lisansı nasıl kuracağınızı gösterir.

````
 ```

// License sınıfını başlat
License license = new License();
// .lic dosyasının yolunu ayarla
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [License()](#License--) | Yeni bir [License](../../com.groupdocs.parser.licensing/license) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Bileşeni lisanslar. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Bileşeni lisanslar. |
|
### License() {#License--}
```
public License()
```


Yeni bir [License](../../com.groupdocs.parser.licensing/license) sınıfı örneği başlatır.


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Bileşeni lisanslar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Lisans dosyasının mutlak yolu. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Bileşeni lisanslar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.InputStream | Lisans akışı. |
|

