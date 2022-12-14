---
title: RawPageCount
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Ruft die Gesamtzahl der Rohseiten des Dokuments ab.
type: docs
weight: 40
url: /de/net/groupdocs.parser.options/documentinfo/rawpagecount/
---
## DocumentInfo.RawPageCount property

Ruft die Gesamtzahl der Rohseiten des Dokuments ab.

```csharp
public int RawPageCount { get; }
```

### Eigentumswert

Ein ganzzahliger Wert, der eine Gesamtzahl von Raw-Seiten darstellt.

### Bemerkungen

verwenden`RawPageCount` Eigentum statt[`PageCount`](../pagecount) Eigenschaft für die Rohtextextraktion. Einige Dokumente haben unterschiedliche Seitenzahlen im genauen und im Rohtextextraktionsmodus. [`PageCount`](../pagecount)-Eigenschaft kann zusätzliche Berechnungen durchführen, die sich auf die Textextraktionsgeschwindigkeit im Rohmodus auswirken.

### Siehe auch

* class [DocumentInfo](../../documentinfo)
* namensraum [GroupDocs.Parser.Options](../../documentinfo)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
