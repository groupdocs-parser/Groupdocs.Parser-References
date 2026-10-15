---
title: "PreviewOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen."
type: docs
weight: 550
url: /de/net/groupdocs.parser.options/previewoptions/
---

## PreviewOptions class

Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen.

```csharp
public class PreviewOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Initialisiert eine neue Instanz der [`PreviewOptions`](../previewoptions)-Klasse, wodurch der Ausgabestream geschlossen wird. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Initialisiert eine neue Instanz der [`PreviewOptions`](../previewoptions)-Klasse, wodurch der Ausgabestream an den Client zurückgegeben wird für weitere Verwendung. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CreatePageStream](../../groupdocs.parser.options/previewoptions/createpagestream) { get; set; } | Liest oder setzt eine Instanz des Delegaten zur Erstellung des Seitenstreams. |
| [Dpi](../../groupdocs.parser.options/previewoptions/dpi) { get; set; } | Liest oder setzt einen DPI-Wert. |
| [Height](../../groupdocs.parser.options/previewoptions/height) { get; set; } | Liest oder setzt die Höhe der Seitenvorschau. |
| [PageNumbers](../../groupdocs.parser.options/previewoptions/pagenumbers) { get; set; } | Liest oder setzt ein Array von Seitenzahlen, für die Vorschauen erzeugt werden. |
| [PreviewFormat](../../groupdocs.parser.options/previewoptions/previewformat) { get; set; } | Liest oder setzt das Bildformat der Vorschau. |
| [PreviewPageRender](../../groupdocs.parser.options/previewoptions/previewpagerender) { get; set; } | Liest oder setzt eine Instanz des Delegaten für Renderinformationen der Seitenvorschau. |
| [ReleasePageStream](../../groupdocs.parser.options/previewoptions/releasepagestream) { get; set; } | Liest oder setzt eine Instanz des Delegaten für den Abschluss der Seitenvorschau. |
| [Width](../../groupdocs.parser.options/previewoptions/width) { get; set; } | Liest oder setzt die Breite der Seitenvorschau. |

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
