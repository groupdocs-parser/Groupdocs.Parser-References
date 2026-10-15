---
title: "IDocumentInfo"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Dokumentinformationen dar."
type: docs
weight: 370
url: /de/net/groupdocs.parser.options/idocumentinfo/
---

## IDocumentInfo interface

Stellt die Dokumentinformationen dar.

```csharp
public interface IDocumentInfo
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | Gibt den Dokumenttyp zurück. |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | Ruft die Gesamtzahl der Dokumentseiten ab. |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | Ruft Informationen über Seiten ab, wie den Index und die Seitengröße. |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | Ruft die Gesamtzahl der rohen Dokumentseiten ab. |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | Gibt die Größe des Dokuments in Bytes zurück. |

### Hinweise

Die Objekte, die dieses Interface implementieren, werden von der Methode [`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo) zurückgegeben. Siehe dort die Anwendungsbeispiele. **Mehr erfahren:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
