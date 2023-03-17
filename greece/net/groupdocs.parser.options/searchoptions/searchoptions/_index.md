---
title: SearchOptions
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Αρχικοποιεί μια νέα παρουσία τουSearchOptionsgroupdocs.parser.options/searchoptions τάξη.
type: docs
weight: 10
url: /el/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία του[`SearchOptions`](../../searchoptions) τάξη.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν δεν αγνοείται μια περίπτωση κειμένου. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται από μια ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| searchByPages | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση πραγματοποιείται ανά σελίδες. |
| leftHighlightOptions | HighlightOptions | Οι επιλογές για την αριστερή επισήμανση. |
| rightHighlightOptions | HighlightOptions | Οι επιλογές για τη σωστή επισήμανση. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../searchoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία του[`SearchOptions`](../../searchoptions) κλάση που χρησιμοποιείται για την αναζήτηση με τις επιλογές επισήμανσης για την αριστερή και τη δεξιά εξαγωγή επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν δεν αγνοείται μια περίπτωση κειμένου. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται από μια ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| leftHighlightOptions | HighlightOptions | Οι επιλογές για την αριστερή επισήμανση. |
| rightHighlightOptions | HighlightOptions | Οι επιλογές για τη σωστή επισήμανση. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../searchoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία του[`SearchOptions`](../../searchoptions) κλάση που χρησιμοποιείται για την αναζήτηση με τις ίδιες επιλογές επισήμανσης για την εξαγωγή αριστερά και δεξιά.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν δεν αγνοείται μια περίπτωση κειμένου. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται από μια ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| highlightOptions | HighlightOptions | Οι επιλογές και για τα δύο highlights. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../searchoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`SearchOptions`](../../searchoptions) κλάση που χρησιμοποιείται για αναζήτηση χωρίς εξαγωγή επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν δεν αγνοείται μια περίπτωση κειμένου. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται από μια ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |

### Δείτε επίσης

* class [SearchOptions](../../searchoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../searchoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`SearchOptions`](../../searchoptions)κλάση που χρησιμοποιείται για αναζήτηση κατά σελίδες και χωρίς εξαγωγή επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν δεν αγνοείται μια περίπτωση κειμένου. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται από μια ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| searchByPages | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση πραγματοποιείται ανά σελίδες. |

### Δείτε επίσης

* class [SearchOptions](../../searchoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../searchoptions)
* συνέλευση [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`SearchOptions`](../../searchoptions) κλάση με προεπιλεγμένες τιμές. Δείτε τις παρατηρήσεις για λεπτομέρειες.

```csharp
public SearchOptions()
```

### Παρατηρήσεις

Οι ακόλουθες ιδιότητες έχουν προεπιλεγμένες τιμές:

**[`MatchCase`](../matchcase)**

`ψευδής`

**[`MatchWholeWord`](../matchwholeword)**

`ψευδής`

**[`UseRegularExpression`](../useregularexpression)**

`ψευδής`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`μηδενικό`

**[`RightHighlightOptions`](../righthighlightoptions)**

`μηδενικό`

### Δείτε επίσης

* class [SearchOptions](../../searchoptions)
* χώρος ονομάτων [GroupDocs.Parser.Options](../../searchoptions)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
