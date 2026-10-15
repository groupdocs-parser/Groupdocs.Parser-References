---
title: "RawPageCount"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Ruft die Gesamtzahl der rohen Dokumentseiten ab."
type: docs
weight: 40
url: /de/net/groupdocs.parser.options/documentinfo/rawpagecount/
---

## DocumentInfo.RawPageCount property

Ruft die Gesamtzahl der rohen Dokumentseiten ab.

```csharp
public int RawPageCount { get; }
```

### Property Value

Ein ganzzahliger Wert, der die Gesamtzahl der Rohseiten darstellt.

### Hinweise

Verwenden Sie die `RawPageCount`-Eigenschaft anstelle der [`PageCount`](../pagecount)-Eigenschaft für die Rohtext-Extraktion. Einige Dokumente haben unterschiedliche Seitennummern in den genauen und Rohtext-Extraktionsmodi. Die [`PageCount`](../pagecount)-Eigenschaft kann zusätzliche Berechnungen durchführen, die die Geschwindigkeit der Textextraktion im Rohmodus beeinträchtigen.

### Siehe auch

* class [DocumentInfo](../../documentinfo)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
