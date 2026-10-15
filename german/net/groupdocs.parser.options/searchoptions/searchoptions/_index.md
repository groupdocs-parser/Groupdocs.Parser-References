---
title: "SearchOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Klasse SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initialisiert eine neue Instanz der Klasse [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| searchByPages | Boolean | Der Wert, der angibt, ob die Suche seitenweise durchgeführt wird. |
| leftHighlightOptions | HighlightOptions | Die Optionen für die linke Hervorhebung. |
| rightHighlightOptions | HighlightOptions | Die Optionen für die rechte Hervorhebung. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Initialisiert eine neue Instanz der Klasse [`SearchOptions`](../../searchoptions) mit dem Seitenlimit.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| maxPageIndex | Int32 | Der Wert, der angibt, ob die Suche seitenweise durchgeführt wird. |
| leftHighlightOptions | HighlightOptions | Die Optionen für die linke Hervorhebung. |
| rightHighlightOptions | HighlightOptions | Die Optionen für die rechte Hervorhebung. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initialisiert eine neue Instanz der Klasse [`SearchOptions`](../../searchoptions), die verwendet wird, um mit den Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| leftHighlightOptions | HighlightOptions | Die Optionen für die linke Hervorhebung. |
| rightHighlightOptions | HighlightOptions | Die Optionen für die rechte Hervorhebung. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initialisiert eine neue Instanz der Klasse [`SearchOptions`](../../searchoptions), die verwendet wird, um mit denselben Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| highlightOptions | HighlightOptions | Die Optionen für beide Hervorhebungen. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initialisiert eine neue Instanz der [`SearchOptions`](../../searchoptions) Klasse, die verwendet wird, um ohne Hervorhebungs-Extraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |

### Siehe auch

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initialisiert eine neue Instanz der [`SearchOptions`](../../searchoptions) Klasse, die verwendet wird, um nach Seiten zu suchen und ohne Hervorhebungs-Extraktion.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| searchByPages | Boolean | Der Wert, der angibt, ob die Suche seitenweise durchgeführt wird. |

### Siehe auch

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initialisiert eine neue Instanz der [`SearchOptions`](../../searchoptions) Klasse mit Standardwerten. Siehe Anmerkungen für Details.

```csharp
public SearchOptions()
```

### Hinweise

Die folgenden Eigenschaften haben Standardwerte:

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

### Siehe auch

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
