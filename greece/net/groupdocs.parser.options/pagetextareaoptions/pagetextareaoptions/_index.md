---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions με την επιλογή χρήσης OCR."
type: docs
weight: 10
url: /el/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με την επιλογή χρήσης OCR.

```csharp
public PageTextAreaOptions()
```

### Δείτε επίσης

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με την επιλογή χρήσης OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| useOcr | Boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή περιοχών κειμένου. |

### Δείτε επίσης

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με τη δυνατότητα ορισμού επιλογών OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| useOcr | Boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή περιοχών κειμένου. |
| ocrOptions | OcrOptions | Οι πρόσθετες επιλογές για τη λειτουργία OCR. |

### Δείτε επίσης

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με την κανονική έκφραση. Οι άλλες επιλογές ορίζονται εξ ορισμού (δείτε τις παρατηρήσεις για λεπτομέρειες).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |

### Σχόλια

Οι παρακάτω ιδιότητες έχουν προεπιλεγμένες τιμές:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### Δείτε επίσης

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με την κανονική έκφραση και το ορθογώνιο πεδίο. Οι άλλες επιλογές ορίζονται εξ ορισμού (δείτε τις παρατηρήσεις για λεπτομέρειες).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |
| rectangle | Rectangle | Η ορθογώνια περιοχή που περιέχει περιοχές σελίδας. |

### Σχόλια

Οι παρακάτω ιδιότητες έχουν προεπιλεγμένες τιμές:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### Δείτε επίσης

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με την κανονική έκφραση, το ορθογώνιο πεδίο και το μέγεθος του αγνοημένου περιγράμματος. Οι άλλες επιλογές ορίζονται εξ ορισμού (δείτε τις παρατηρήσεις για λεπτομέρειες).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |
| rectangle | Rectangle | Η ορθογώνια περιοχή που περιέχει περιοχές σελίδας. |
| rectangleTolerance | Double | Το μέγεθος του περιθωρίου που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετράται ως κλάσμα του ύψους ενός στοιχείου κειμένου. |

### Δείτε επίσης

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions).

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| uniteSegments | Boolean | Η τιμή που υποδεικνύει εάν τα τμήματα ενώνται. |
| ignoreFormatting | Boolean | Η τιμή που υποδεικνύει εάν η μορφοποίηση κειμένου αγνοείται. |
| rectangle | Rectangle | Η ορθογώνια περιοχή που περιέχει περιοχές σελίδας. |

### Δείτε επίσης

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageTextAreaOptions`](../../pagetextareaoptions) με το μέγεθος του αγνοημένου περιγράμματος.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| uniteSegments | Boolean | Η τιμή που υποδεικνύει εάν τα τμήματα ενώνται. |
| ignoreFormatting | Boolean | Η τιμή που υποδεικνύει εάν η μορφοποίηση κειμένου αγνοείται. |
| rectangle | Rectangle | Η ορθογώνια περιοχή που περιέχει περιοχές σελίδας. |
| rectangleTolerance | Double | Το μέγεθος του περιθωρίου που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετράται ως κλάσμα του ύψους ενός στοιχείου κειμένου. |

### Δείτε επίσης

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
