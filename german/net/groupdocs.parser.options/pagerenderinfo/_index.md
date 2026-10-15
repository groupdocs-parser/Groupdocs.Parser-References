---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Informationen darüber dar, wie eine Seite gerendert wird."
type: docs
weight: 500
url: /de/net/groupdocs.parser.options/pagerenderinfo/
---

## PageRenderInfo class

Stellt die Informationen darüber dar, wie eine Seite gerendert wird.

```csharp
public sealed class PageRenderInfo
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageRenderInfo](pagerenderinfo)(int, int, int) | Initialisiert eine neue Instanz der [`PageRenderInfo`](../pagerenderinfo)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ColumnCount](../../groupdocs.parser.options/pagerenderinfo/columncount) { get; } | Ermittelt die Gesamtzahl der Kachelspalten. |
| [PageNumber](../../groupdocs.parser.options/pagerenderinfo/pagenumber) { get; } | Ermittelt die Seitennummer. |
| [RowCount](../../groupdocs.parser.options/pagerenderinfo/rowcount) { get; } | Ermittelt die Gesamtzahl der Kachelzeilen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetColumn](../../groupdocs.parser.options/pagerenderinfo/getcolumn)(int) | Gibt den Index der Spalte zurück, in der die Kachel mit *tileIndex* platziert ist. |
| [GetRow](../../groupdocs.parser.options/pagerenderinfo/getrow)(int) | Gibt den Index der Zeile zurück, in der die Kachel mit *tileIndex* platziert ist. |

### Hinweise

Einige Dokumente (z. B. Tabellenkalkulationen) können nicht als einzelnes Bild gerendert werden. Für diese Dokumente wird eine Seite als Satz von Kacheln gerendert. Diese Kacheln werden in einer rechteckigen Tabelle angeordnet.

[`RowCount`](./rowcount) and [`ColumnCount`](./columncount) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
