---
title: "License"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει την άδεια του GroupDocs.Parser."
type: docs
weight: 10
url: /el/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Αντιπροσωπεύει την άδεια του GroupDocs.Parser.

Αυτό το παράδειγμα δείχνει πώς να ρυθμίσετε την άδεια.

````
 ```

// Αρχικοποίηση κλάσης License
License license = new License();
// Ορίστε τη διαδρομή στο αρχείο .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [License()](#License--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [License](../../com.groupdocs.parser.licensing/license). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Παρέχει άδεια στο στοιχείο. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Παρέχει άδεια στο στοιχείο. |
|
### License() {#License--}
```
public License()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Παρέχει άδεια στο στοιχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Απόλυτη διαδρομή στο αρχείο άδειας. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Παρέχει άδεια στο στοιχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | stream | java.io.InputStream | Ροή άδειας. |
|

