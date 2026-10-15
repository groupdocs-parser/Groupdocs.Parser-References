---
title: "DocumentPageData"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt Daten der Dokumentseite dar. Sie besteht aus FieldData./fielddata‑Objekten, die Felddaten der Dokumentseite enthalten."
type: docs
weight: 740
url: /de/net/groupdocs.parser.data/documentpagedata/
---

## DocumentPageData class

Stellt Daten der Dokumentseite dar. Sie besteht aus [`FieldData`](../fielddata)-Objekten, die Felddaten der Dokumentseite enthalten.

```csharp
public sealed class DocumentPageData : DocumentData
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Gibt die Gesamtzahl der Felddaten zurück. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Gibt die Felddaten anhand eines Index zurück. |
| [PageIndex](../../groupdocs.parser.data/documentpagedata/pageindex) { get; } | Liefert den Seitenindex. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Gibt die Vorlage zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Gibt einen Enumerator für die Felddaten zurück. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Gibt die Sammlung von Felddaten zurück, bei denen der Name gleich *fieldName* ist. |

### Siehe auch

* class [DocumentData](../documentdata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
