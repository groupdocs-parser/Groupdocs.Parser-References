---
title: "PageImageArea"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt einen Seiten-Bild-Bereich dar, der verwendet wird, um ein Bild auf der Seite in der Vorlagen-Parsing-Funktionalität oder einen Bildanhang zu repräsentieren, wenn Bilder aus E-Mails oder Zip-Archiven extrahiert werden."
type: docs
weight: 830
url: /de/net/groupdocs.parser.data/pageimagearea/
---

## PageImageArea class

Stellt einen Seiten-Bild-Bereich dar, der verwendet wird, um ein Bild auf der Seite in der Vorlagen-Parsing-Funktionalität oder einen Bildanhang zu repräsentieren, wenn Bilder aus E-Mails oder Zip-Archiven extrahiert werden.

```csharp
public sealed class PageImageArea : PageArea
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | Initialisiert eine neue Instanz der [`PageImageArea`](../pageimagearea)-Klasse. |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | Initialisiert eine neue Instanz der [`PageImageArea`](../pageimagearea)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | Liefert das Format des Bildes. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Liefert die Dokumentseiteninformationen wie Seitenindex und Seitengröße. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Liefert den rechteckigen Bereich. |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | Liefert den Rotationswinkel des Bildes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | Gibt den Bild-Stream zurück. |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | Gibt den Bild-Stream in einem anderen Format zurück. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | Speichert das Bild in die Datei. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | Speichert das Bild in die Datei in einem anderen Format. |

### Hinweise

Eine Instanz der [`PageImageArea`](../pageimagearea)-Klasse wird als Rückgabewert der folgenden Methoden verwendet:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

Siehe dort die Anwendungsbeispiele.

### Siehe auch

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
