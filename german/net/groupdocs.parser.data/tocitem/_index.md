---
title: "TocItem"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt das Element dar, das in der Inhaltsverzeichnis-Extraktionsfunktion verwendet wird."
type: docs
weight: 920
url: /de/net/groupdocs.parser.data/tocitem/
---

## TocItem class

Stellt das Element dar, das in der Inhaltsverzeichnis-Extraktionsfunktion verwendet wird.

```csharp
public class TocItem
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TocItem](tocitem)(int, string, int?) | Initialisiert eine neue Instanz der Klasse [`TocItem`](../tocitem). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Depth](../../groupdocs.parser.data/tocitem/depth) { get; } | Liefert die Ebenentiefe. |
| [PageIndex](../../groupdocs.parser.data/tocitem/pageindex) { get; } | Liefert den Seitenindex. |
| [Text](../../groupdocs.parser.data/tocitem/text) { get; } | Liefert den Text. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [ExtractText](../../groupdocs.parser.data/tocitem/extracttext)() | Extrahiert einen Text aus dem Dokument, auf den das Objekt [`TocItem`](../tocitem) verweist. |

### Hinweise

Eine Instanz der Klasse [`TocItem`](../tocitem) wird als Rückgabewert der Methode [`GetToc`](../../groupdocs.parser/parser/gettoc) verwendet. Siehe dort die Anwendungsbeispiele.

### Siehe auch

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
