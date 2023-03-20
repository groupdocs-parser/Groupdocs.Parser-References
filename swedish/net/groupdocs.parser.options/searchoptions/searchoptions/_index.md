---
title: SearchOptions
second_title: GroupDocs.Parser för .NET API-referens
description: Initierar en ny instans avSearchOptionsgroupdocs.parser.options/searchoptions class.
type: docs
weight: 10
url: /sv/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initierar en ny instans av[`SearchOptions`](../../searchoptions) class.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| matchCase | Boolean | Värdet som indikerar om ett skiftläge för text inte ignoreras. |
| matchWholeWord | Boolean | Värdet som anger om textsökning är begränsad av ett helt ord. |
| useRegularExpression | Boolean | Värdet som anger om ett reguljärt uttryck används. |
| searchByPages | Boolean | Värdet som anger om sökningen utförs av sidor. |
| leftHighlightOptions | HighlightOptions | Alternativen för vänster markering. |
| rightHighlightOptions | HighlightOptions | Alternativen för rätt markering. |

### Se även

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namnutrymme [GroupDocs.Parser.Options](../../searchoptions)
* hopsättning [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initierar en ny instans av[`SearchOptions`](../../searchoptions) klass som används för att söka med markeringsalternativen för vänster och höger högdagerextraktion.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| matchCase | Boolean | Värdet som indikerar om ett skiftläge för text inte ignoreras. |
| matchWholeWord | Boolean | Värdet som anger om textsökning är begränsad av ett helt ord. |
| useRegularExpression | Boolean | Värdet som anger om ett reguljärt uttryck används. |
| leftHighlightOptions | HighlightOptions | Alternativen för vänster markering. |
| rightHighlightOptions | HighlightOptions | Alternativen för rätt markering. |

### Se även

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namnutrymme [GroupDocs.Parser.Options](../../searchoptions)
* hopsättning [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initierar en ny instans av[`SearchOptions`](../../searchoptions) klass som används för att söka med samma markeringsalternativ för vänster- och högermarkeringsextraktion.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| matchCase | Boolean | Värdet som indikerar om ett skiftläge för text inte ignoreras. |
| matchWholeWord | Boolean | Värdet som anger om textsökning är begränsad av ett helt ord. |
| useRegularExpression | Boolean | Värdet som anger om ett reguljärt uttryck används. |
| highlightOptions | HighlightOptions | Alternativen för båda höjdpunkterna. |

### Se även

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namnutrymme [GroupDocs.Parser.Options](../../searchoptions)
* hopsättning [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initierar en ny instans av[`SearchOptions`](../../searchoptions) klass som används för att söka utan markering.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| matchCase | Boolean | Värdet som indikerar om ett skiftläge för text inte ignoreras. |
| matchWholeWord | Boolean | Värdet som anger om textsökning är begränsad av ett helt ord. |
| useRegularExpression | Boolean | Värdet som anger om ett reguljärt uttryck används. |

### Se även

* class [SearchOptions](../../searchoptions)
* namnutrymme [GroupDocs.Parser.Options](../../searchoptions)
* hopsättning [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initierar en ny instans av[`SearchOptions`](../../searchoptions)klass som används för att söka efter sidor och utan markering.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| matchCase | Boolean | Värdet som indikerar om ett skiftläge för text inte ignoreras. |
| matchWholeWord | Boolean | Värdet som anger om textsökning är begränsad av ett helt ord. |
| useRegularExpression | Boolean | Värdet som anger om ett reguljärt uttryck används. |
| searchByPages | Boolean | Värdet som anger om sökningen utförs av sidor. |

### Se även

* class [SearchOptions](../../searchoptions)
* namnutrymme [GroupDocs.Parser.Options](../../searchoptions)
* hopsättning [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initierar en ny instans av[`SearchOptions`](../../searchoptions) klass med standardvärden. Se kommentarer för detaljer.

```csharp
public SearchOptions()
```

### Anmärkningar

Följande egenskaper har standardvärden:

**[`MatchCase`](../matchcase)**

`falsk`

**[`MatchWholeWord`](../matchwholeword)**

`falsk`

**[`UseRegularExpression`](../useregularexpression)**

`falsk`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### Se även

* class [SearchOptions](../../searchoptions)
* namnutrymme [GroupDocs.Parser.Options](../../searchoptions)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
