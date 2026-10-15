---
title: "HighlightOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die verwendet werden, um einen hervorgehobenen Textblock um gefundenen Text in Suchszenarien zu extrahieren."
type: docs
weight: 360
url: /de/net/groupdocs.parser.options/highlightoptions/
---

## HighlightOptions class

Stellt die Optionen bereit, die zum Extrahieren einer Hervorhebung (eines Textblocks um gefundenen Text in Suchszenarien) verwendet werden.

```csharp
public sealed class HighlightOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)() | Initialisiert eine neue Instanz der [`HighlightOptions`](../highlightoptions)-Klasse, die verwendet wird, um ein Highlight mit fester Länge zu extrahieren. |
| [HighlightOptions](highlightoptions#constructor_1)(int) | Initialisiert eine neue Instanz der [`HighlightOptions`](../highlightoptions)-Klasse, die verwendet wird, um ein Highlight mit fester Länge zu extrahieren. |
| [HighlightOptions](highlightoptions#constructor_2)(int?, bool) | Initialisiert eine neue Instanz der [`HighlightOptions`](../highlightoptions)-Klasse, die verwendet wird, um ein zeilenbegrenztes Highlight zu extrahieren. |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int) | Initialisiert eine neue Instanz der [`HighlightOptions`](../highlightoptions)-Klasse, die verwendet wird, um ein Highlight mit fester Wortanzahl zu extrahieren. |
| [HighlightOptions](highlightoptions#constructor_4)(int?, int?, bool) | Initialisiert eine neue Instanz der [`HighlightOptions`](../highlightoptions)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; set; } | Ermittelt den Wert, der angibt, ob die Highlight-Extraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist. |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; set; } | Ermittelt eine maximale Textlänge. |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; set; } | Ermittelt eine maximale Wortanzahl. |

### Hinweise

Eine Instanz der Klasse [`HighlightOptions`](../highlightoptions) wird als Parameter in der Methode [`GetHighlight`](../../groupdocs.parser/parser/gethighlight) verwendet. Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
