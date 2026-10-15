---
title: "LoadOptions"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης LoadOptionsgroupdocs.parser.options/loadoptions με κενό Passwordgroupdocs.parser.options/loadoptions/password, FileFormatgroupdocs.parser.options/loadoptions/fileformat ίσο με Unknown και προεπιλεγμένες κωδικοποιήσεις."
type: docs
weight: 10
url: /el/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με κενό [`Password`](../password), [`FileFormat`](../fileformat) ίσο με Unknown και προεπιλεγμένες κωδικοποιήσεις.

```csharp
public LoadOptions()
```

### Δείτε επίσης

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| timeout | TimeSpan | Το TimeSpan που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |

### Δείτε επίσης

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με [`FileFormat`](../fileformat) ίσο με Unknown και προεπιλεγμένες κωδικοποιήσεις.

```csharp
public LoadOptions(string password)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |

### Δείτε επίσης

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με κενό [`Password`](../password) και προεπιλεγμένες κωδικοποιήσεις.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileFormat | FileFormat | Η μορφή του αρχείου. |

### Δείτε επίσης

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με τον κωδικό πρόσβασης και προεπιλεγμένες κωδικοποιήσεις.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileFormat | FileFormat | Η μορφή του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |

### Δείτε επίσης

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με προσαρμοσμένες κωδικοποιήσεις.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileFormat | FileFormat | Η μορφή του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
| encoding | Encoding | Η κωδικοποίηση του εγγράφου. |
| defaultAnsiEncoding | Encoding | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |

### Δείτε επίσης

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) πλήρως προσαρμοσμένης.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileFormat | FileFormat | Η μορφή του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
| encoding | Encoding | Η κωδικοποίηση του εγγράφου. |
| defaultAnsiEncoding | Encoding | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
| timeout | TimeSpan | Το TimeSpan που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |

### Δείτε επίσης

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με κενό [`Password`](../password) και προεπιλεγμένες κωδικοποιήσεις.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileType | FileType | Ο τύπος του αρχείου. |

### Δείτε επίσης

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με τον κωδικό πρόσβασης και προεπιλεγμένες κωδικοποιήσεις.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileType | FileType | Ο τύπος του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |

### Δείτε επίσης

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) με προσαρμοσμένες κωδικοποιήσεις.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileType | FileType | Ο τύπος του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
| encoding | Encoding | Η κωδικοποίηση του εγγράφου. |
| defaultAnsiEncoding | Encoding | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |

### Δείτε επίσης

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LoadOptions`](../../loadoptions) πλήρως προσαρμοσμένης.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| fileType | FileType | Ο τύπος του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
| encoding | Encoding | Η κωδικοποίηση του εγγράφου. |
| defaultAnsiEncoding | Encoding | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
| timeout | TimeSpan | Το TimeSpan που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |

### Δείτε επίσης

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
