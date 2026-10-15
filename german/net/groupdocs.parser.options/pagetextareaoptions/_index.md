---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion von Textbereichen auf Seiten verwendet werden."
type: docs
weight: 520
url: /de/net/groupdocs.parser.options/pagetextareaoptions/
---

## PageTextAreaOptions class

Stellt die Optionen bereit, die für die Extraktion von Textbereichen auf Seiten verwendet werden.

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)() | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit der OCR‑Verwendungsoption. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit der OCR‑Verwendungsoption. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit dem regulären Ausdruck. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(bool, OcrOptions) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit der Möglichkeit, OCR‑Optionen festzulegen. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_6)(string, Rectangle) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit dem regulären Ausdruck und dem rechteckigen Bereich. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_7)(string, Rectangle, double) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit dem regulären Ausdruck, dem rechteckigen Bereich und der Größe des zu ignorierenden Randes. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, bool, bool, bool, Rectangle) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_5)(string, bool, bool, bool, Rectangle, double) | Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../pagetextareaoptions)-Klasse mit der Größe des zu ignorierenden Randes. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; set; } | Ermittelt den regulären Ausdruck. |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; set; } | Ermittelt den Wert, der angibt, ob die Textformatierung ignoriert wird. |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; set; } | Ermittelt den Wert, der angibt, ob die Groß-/Kleinschreibung des Textes nicht ignoriert wird. |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; set; } | Gibt die zusätzlichen Optionen für die OCR-Funktionalität zurück. |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Liest den rechteckigen Bereich, der Seitenbereiche enthält. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Liest die Größe des Randes, der beim Erfassen durch den rechteckigen Bereich ignoriert wird. Er wird als Bruchteil der Höhe eines Textelements gemessen. |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; set; } | Ermittelt den Wert, der angibt, ob Segmente vereinigt werden. |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; set; } | Ruft den Wert ab, der angibt, ob die OCR‑Funktionalität zum Extrahieren von Textbereichen verwendet wird. |

### Hinweise

Eine Instanz der Klasse [`PageTextAreaOptions`](../pagetextareaoptions) wird als Parameter in den Methoden [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) und [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) verwendet. Siehe dort die Anwendungsbeispiele. **Erfahren Sie mehr:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Siehe auch

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
