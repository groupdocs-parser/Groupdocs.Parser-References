---
title: "SearchOptions"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Initialiseert een nieuwe instantie van de SearchOptionsgroupdocs.parser.options/searchoptions klasse."
type: docs
weight: 10
url: /nl/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initialiseert een nieuwe instantie van de [`SearchOptions`](../../searchoptions) klasse.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekst zoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| searchByPages | Boolean | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |
| leftHighlightOptions | HighlightOptions | De opties voor de linker markering. |
| rightHighlightOptions | HighlightOptions | De opties voor de rechter markering. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Initialiseert een nieuw exemplaar van de [`SearchOptions`](../../searchoptions) klasse met de paginalimiet.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekst zoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| maxPageIndex | Int32 | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |
| leftHighlightOptions | HighlightOptions | De opties voor de linker markering. |
| rightHighlightOptions | HighlightOptions | De opties voor de rechter markering. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initialiseert een nieuw exemplaar van de [`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om te zoeken met de markeeropties voor de linker- en rechtermarkeringsextractie.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekst zoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| leftHighlightOptions | HighlightOptions | De opties voor de linker markering. |
| rightHighlightOptions | HighlightOptions | De opties voor de rechter markering. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initialiseert een nieuw exemplaar van de [`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om te zoeken met dezelfde markeeropties voor de linker- en rechtermarkeringsextractie.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekst zoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| highlightOptions | HighlightOptions | De opties voor beide markeringen. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om te zoeken zonder markeringsextractie.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekst zoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |

### Zie ook

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om per pagina te zoeken en zonder markeringsextractie.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekst zoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| searchByPages | Boolean | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |

### Zie ook

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initialiseert een nieuw exemplaar van de [`SearchOptions`](../../searchoptions) klasse met standaardwaarden. Zie opmerkingen voor details.

```csharp
public SearchOptions()
```

### Opmerkingen

De volgende eigenschappen hebben standaardwaarden:

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

### Zie ook

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
