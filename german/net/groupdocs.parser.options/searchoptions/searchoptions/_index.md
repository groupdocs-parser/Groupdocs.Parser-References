---
title: SearchOptions
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Initialisiert eine neue Instanz vonSearchOptionsgroupdocs.parser.options/searchoptions Klasse.
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initialisiert eine neue Instanz von[`SearchOptions`](../../searchoptions) Klasse.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| searchByPages | Boolean | Der Wert, der angibt, ob die Suche nach Seiten durchgeführt wird. |
| leftHighlightOptions | HighlightOptions | Die Optionen für die linke Markierung. |
| rightHighlightOptions | HighlightOptions | Die Optionen für das richtige Highlight. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namensraum [GroupDocs.Parser.Options](../../searchoptions)
* Montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initialisiert eine neue Instanz von[`SearchOptions`](../../searchoptions) Klasse, die verwendet wird, um mit den Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| leftHighlightOptions | HighlightOptions | Die Optionen für die linke Markierung. |
| rightHighlightOptions | HighlightOptions | Die Optionen für das richtige Highlight. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namensraum [GroupDocs.Parser.Options](../../searchoptions)
* Montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initialisiert eine neue Instanz von[`SearchOptions`](../../searchoptions) Klasse, die verwendet wird, um mit denselben Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| highlightOptions | HighlightOptions | Die Optionen für beide Highlights. |

### Siehe auch

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namensraum [GroupDocs.Parser.Options](../../searchoptions)
* Montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initialisiert eine neue Instanz von[`SearchOptions`](../../searchoptions) Klasse, die verwendet wird, um ohne Highlight-Extraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |

### Siehe auch

* class [SearchOptions](../../searchoptions)
* namensraum [GroupDocs.Parser.Options](../../searchoptions)
* Montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initialisiert eine neue Instanz von[`SearchOptions`](../../searchoptions)Klasse, die verwendet wird, um nach Seiten und ohne Highlight-Extraktion zu suchen.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| matchCase | Boolean | Der Wert, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| matchWholeWord | Boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| useRegularExpression | Boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
| searchByPages | Boolean | Der Wert, der angibt, ob die Suche nach Seiten durchgeführt wird. |

### Siehe auch

* class [SearchOptions](../../searchoptions)
* namensraum [GroupDocs.Parser.Options](../../searchoptions)
* Montage [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initialisiert eine neue Instanz von[`SearchOptions`](../../searchoptions) Klasse mit Standardwerten. Siehe Bemerkungen für Details.

```csharp
public SearchOptions()
```

### Bemerkungen

Die folgenden Eigenschaften haben Standardwerte:

**[`MatchCase`](../matchcase)**

`FALSCH`

**[`MatchWholeWord`](../matchwholeword)**

`FALSCH`

**[`UseRegularExpression`](../useregularexpression)**

`FALSCH`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`Null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`Null`

### Siehe auch

* class [SearchOptions](../../searchoptions)
* namensraum [GroupDocs.Parser.Options](../../searchoptions)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
