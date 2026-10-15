---
title: "SearchOptions"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αρχικοποιεί ένα νέο αντικείμενο της κλάσης SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /el/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| searchByPages | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες. |
| leftHighlightOptions | HighlightOptions | Οι επιλογές για την αριστερή επισήμανση. |
| rightHighlightOptions | HighlightOptions | Οι επιλογές για τη δεξιά επισήμανση. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SearchOptions`](../../searchoptions) με το όριο σελίδων.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| maxPageIndex | Int32 | Η τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες. |
| leftHighlightOptions | HighlightOptions | Οι επιλογές για την αριστερή επισήμανση. |
| rightHighlightOptions | HighlightOptions | Οι επιλογές για τη δεξιά επισήμανση. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SearchOptions`](../../searchoptions) που χρησιμοποιείται για αναζήτηση με τις επιλογές επισήμανσης για την εξαγωγή της αριστερής και της δεξιάς επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| leftHighlightOptions | HighlightOptions | Οι επιλογές για την αριστερή επισήμανση. |
| rightHighlightOptions | HighlightOptions | Οι επιλογές για τη δεξιά επισήμανση. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SearchOptions`](../../searchoptions) που χρησιμοποιείται για αναζήτηση με τις ίδιες επιλογές επισήμανσης για την εξαγωγή της αριστερής και της δεξιάς επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| highlightOptions | HighlightOptions | Οι επιλογές και για τις δύο επισήμανσεις. |

### Δείτε επίσης

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SearchOptions`](../../searchoptions) που χρησιμοποιείται για αναζήτηση χωρίς εξαγωγή επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |

### Δείτε επίσης

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SearchOptions`](../../searchoptions) που χρησιμοποιείται για αναζήτηση ανά σελίδες και χωρίς εξαγωγή επισήμανσης.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| matchCase | Boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
| matchWholeWord | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
| useRegularExpression | Boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
| searchByPages | Boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες. |

### Δείτε επίσης

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SearchOptions`](../../searchoptions) με προεπιλεγμένες τιμές. Δείτε τις παρατηρήσεις για λεπτομέρειες.

```csharp
public SearchOptions()
```

### Σχόλια

Οι παρακάτω ιδιότητες έχουν προεπιλεγμένες τιμές:

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### Δείτε επίσης

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
