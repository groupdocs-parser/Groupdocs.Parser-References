---
title: "TextReader"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل قارئًا يمكنه قراءة سلسلة متسلسلة من الأحرف."
type: docs
weight: 29
url: /ar/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

يمثل قارئًا يمكنه قراءة سلسلة متسلسلة من الأحرف.

## البناؤات

| البناء | الوصف |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | يقرأ سطرًا من الأحرف من القارئ النصي ويعيد البيانات كسلسلة. |
|
|  | [readToEnd()](#readToEnd--) | يقرأ جميع الأحرف من الموضع الحالي حتى نهاية القارئ النصي ويعيدها كسلسلة واحدة. |
|
|  | [dispose()](#dispose--) | يطلق جميع الموارد المستخدمة بواسطة كائن [TextReader](../../com.groupdocs.parser.data/textreader). |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


يقرأ سطرًا من الأحرف من القارئ النصي ويعيد البيانات كسلسلة.


**Returns:**
java.lang.String - السطر التالي من القارئ، أو  null  إذا تم قراءة جميع الأحرف.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


يقرأ جميع الأحرف من الموضع الحالي حتى نهاية القارئ النصي ويعيدها كسلسلة واحدة.


**Returns:**
java.lang.String - سلسلة تحتوي على جميع الأحرف من الموضع الحالي حتى نهاية القارئ النصي.

### dispose() {#dispose--}
```
public void dispose()
```


يطلق جميع الموارد المستخدمة بواسطة كائن [TextReader](../../com.groupdocs.parser.data/textreader).


