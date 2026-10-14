---
title: "PreviewOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει επιλογές για τον καθορισμό απαιτήσεων και αντιπροσώπων ροής για τη δημιουργία προεπισκόπησης."
type: docs
weight: 34
url: /el/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Παρέχει επιλογές για τον καθορισμό απαιτήσεων και αντιπροσώπων ροής για τη δημιουργία προεπισκόπησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) προκαλώντας το κλείσιμο του ρεύματος εξόδου. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) προκαλώντας την επιστροφή του ρεύματος εξόδου στον πελάτη για περαιτέρω χρήση. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getWidth()](#getWidth--) | Λαμβάνει το πλάτος της προεπισκόπησης σελίδας. |
|
|  | [setWidth(int width)](#setWidth-int-) | Ορίζει το πλάτος της προεπισκόπησης σελίδας. |
|
|  | [getHeight()](#getHeight--) | Λαμβάνει το ύψος της προεπισκόπησης της σελίδας. |
|
|  | [setHeight(int height)](#setHeight-int-) | Ορίζει το ύψος της προεπισκόπησης της σελίδας. |
|
|  | [getDpi()](#getDpi--) | Λαμβάνει ένα dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Ορίζει ένα dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Λαμβάνει έναν πίνακα αριθμών σελίδων για τη δημιουργία προεπισκοπήσεων. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Ορίζει έναν πίνακα αριθμών σελίδων για τη δημιουργία προεπισκοπήσεων. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Λαμβάνει τη μορφή εικόνας προεπισκόπησης. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Ορίζει τη μορφή εικόνας προεπισκόπησης. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Λαμβάνει ένα στιγμιότυπο του αντιπροσώπου δημιουργίας ροής σελίδας. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Ορίζει ένα στιγμιότυπο του αντιπροσώπου δημιουργίας ροής σελίδας. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Λαμβάνει ένα στιγμιότυπο του αντιπροσώπου ολοκλήρωσης προεπισκόπησης σελίδας. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Ορίζει ένα στιγμιότυπο του αντιπροσώπου ολοκλήρωσης προεπισκόπησης σελίδας. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Λαμβάνει ένα στιγμιότυπο του αντιπροσώπου πληροφοριών απόδοσης προεπισκόπησης σελίδας. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Ορίζει ένα στιγμιότυπο του αντιπροσώπου πληροφοριών απόδοσης προεπισκόπησης σελίδας. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) προκαλώντας το κλείσιμο του ρεύματος εξόδου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) προκαλώντας την επιστροφή του ρεύματος εξόδου στον πελάτη για περαιτέρω χρήση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Ειδοποιεί ότι η δημιουργία προεπισκόπησης σελίδας ολοκληρώθηκε και λαμβάνει τη ροή εξόδου. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Λαμβάνει το πλάτος της προεπισκόπησης σελίδας.


**Returns:**
int - Το πλάτος της σελίδας.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Ορίζει το πλάτος της προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | width | int | Το πλάτος της σελίδας. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Λαμβάνει το ύψος της προεπισκόπησης της σελίδας.


**Returns:**
int - Το ύψος της σελίδας.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Ορίζει το ύψος της προεπισκόπησης της σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | height | int | Το ύψος της σελίδας. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Λαμβάνει ένα dpi.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Ορίζει ένα dpi.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dpi | int | Το dpi. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Λαμβάνει έναν πίνακα αριθμών σελίδων για τη δημιουργία προεπισκοπήσεων.


**Returns:**
int[] - Μια συλλογή αριθμών σελίδας.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Ορίζει έναν πίνακα αριθμών σελίδων για τη δημιουργία προεπισκοπήσεων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageNumbers | int[] | Μια συλλογή αριθμών σελίδας. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Λαμβάνει τη μορφή εικόνας προεπισκόπησης.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Ορίζει τη μορφή εικόνας προεπισκόπησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Η μορφή προεπισκόπησης. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Λαμβάνει ένα στιγμιότυπο του αντιπροσώπου δημιουργίας ροής σελίδας.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Ορίζει ένα στιγμιότυπο του αντιπροσώπου δημιουργίας ροής σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Ο delegate δημιουργίας ροής σελίδας. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Λαμβάνει ένα στιγμιότυπο του αντιπροσώπου ολοκλήρωσης προεπισκόπησης σελίδας.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Ορίζει ένα στιγμιότυπο του αντιπροσώπου ολοκλήρωσης προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Ο delegate ολοκλήρωσης προεπισκόπησης σελίδας. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Λαμβάνει ένα στιγμιότυπο του αντιπροσώπου πληροφοριών απόδοσης προεπισκόπησης σελίδας.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Ορίζει ένα στιγμιότυπο του αντιπροσώπου πληροφοριών απόδοσης προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Ο delegate πληροφοριών απόδοσης προεπισκόπησης σελίδας. |
|

