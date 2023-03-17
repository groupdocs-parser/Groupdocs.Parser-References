---
title: PageTextAreaOptions
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Αρχικοποιεί μια νέα παρουσία τουPageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions τάξη με την επιλογή χρήσης OCR.
type: docs
weight: 10
url: /el/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---
## PageTextAreaOptions(bool) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`PageTextAreaOptions`](../../pagetextareaoptions) τάξη με την επιλογή χρήσης OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| useOcr | Boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή περιοχών κειμένου. |

### Δείτε επίσης

* class [PageTextAreaOptions](../../pagetextareaoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../pagetextareaoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`PageTextAreaOptions`](../../pagetextareaoptions) τάξη με δυνατότητα ρύθμισης επιλογών OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| useOcr | Boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή περιοχών κειμένου. |
| ocrOptions | OcrOptions | Οι πρόσθετες επιλογές για λειτουργικότητα OCR. |

### Δείτε επίσης

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../pagetextareaoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`PageTextAreaOptions`](../../pagetextareaoptions) τάξη με την κανονική έκφραση. Άλλες επιλογές έχουν οριστεί από προεπιλογή (δείτε τις παρατηρήσεις για λεπτομέρειες).

```csharp
public PageTextAreaOptions(string expression)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |

### Παρατηρήσεις

Οι ακόλουθες ιδιότητες έχουν προεπιλεγμένες τιμές:

**[`MatchCase`](../matchcase)**

`ψευδής`

**[`UniteSegments`](../unitesegments)**

`ψευδής`

**[`IgnoreFormatting`](../ignoreformatting)**

`ψευδής`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`μηδενικό`

### Δείτε επίσης

* class [PageTextAreaOptions](../../pagetextareaoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../pagetextareaoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία του[`PageTextAreaOptions`](../../pagetextareaoptions) class με την κανονική έκφραση και το ορθογώνιο εμβαδόν. Άλλες επιλογές έχουν οριστεί από προεπιλογή (δείτε τις παρατηρήσεις για λεπτομέρειες).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |
| rectangle | Rectangle | Η ορθογώνια περιοχή που περιέχει περιοχές σελίδας. |

### Παρατηρήσεις

Οι ακόλουθες ιδιότητες έχουν προεπιλεγμένες τιμές:

**[`MatchCase`](../matchcase)**

`ψευδής`

**[`UniteSegments`](../unitesegments)**

`ψευδής`

**[`IgnoreFormatting`](../ignoreformatting)**

`ψευδής`

### Δείτε επίσης

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../pagetextareaoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία του[`PageTextAreaOptions`](../../pagetextareaoptions) τάξη.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| expression | String | Η κανονική έκφραση. |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν δεν αγνοείται μια περίπτωση κειμένου. |
| uniteSegments | Boolean | Η τιμή που υποδεικνύει εάν τα τμήματα είναι ενωμένα. |
| ignoreFormatting | Boolean | Η τιμή που υποδεικνύει εάν η μορφοποίηση κειμένου αγνοείται. |
| rectangle | Rectangle | Η ορθογώνια περιοχή που περιέχει περιοχές σελίδας. |

### Δείτε επίσης

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../pagetextareaoptions)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->