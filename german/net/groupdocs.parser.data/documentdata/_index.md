---
title: "DocumentData"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt Daten des Dokuments dar. Es besteht aus FieldData./fielddata-Objekten, die Felddaten aus dem Dokument enthalten."
type: docs
weight: 730
url: /de/net/groupdocs.parser.data/documentdata/
---

## DocumentData class

Stellt Daten des Dokuments dar. Es besteht aus [`FieldData`](../fielddata)-Objekten, die Felddaten aus dem Dokument enthalten.

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Gibt die Gesamtzahl der Felddaten zurück. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Gibt die Felddaten anhand eines Index zurück. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Gibt die Vorlage zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Gibt einen Enumerator für die Felddaten zurück. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Gibt die Sammlung von Felddaten zurück, bei denen der Name gleich *fieldName* ist. |

### Hinweise

Eine Instanz der [`DocumentData`](../documentdata)-Klasse wird als Rückgabewert der Methoden [`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) und [`ParseForm`](../../groupdocs.parser/parser/parseform) verwendet. Siehe dort die Anwendungsbeispiele.

### Siehe auch

* class [FieldData](../fielddata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
