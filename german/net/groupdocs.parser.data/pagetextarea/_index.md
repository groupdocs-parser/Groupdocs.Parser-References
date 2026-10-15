---
title: "PageTextArea"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt einen Seiten-Text-Bereich dar, der verwendet wird, um einen Textwert in der Vorlagen-Parsing- oder Formular-Parsing-Funktionalität zu repräsentieren."
type: docs
weight: 860
url: /de/net/groupdocs.parser.data/pagetextarea/
---

## PageTextArea class

Stellt einen Seiten-Text-Bereich dar, der verwendet wird, um einen Textwert in der Vorlagen-Parsing- oder Formular-Parsing-Funktionalität zu repräsentieren.

```csharp
public sealed class PageTextArea : PageArea
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | Initialisiert eine neue Instanz der [`PageTextArea`](../pagetextarea)-Klasse. |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | Initialisiert eine neue Instanz der [`PageTextArea`](../pagetextarea)-Klasse. |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | Initialisiert eine neue Instanz der [`PageTextArea`](../pagetextarea)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | Liefert die Sammlung der untergeordneten Textseitenbereiche. |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | Liefert die Grundlinie. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Liefert die Dokumentseiteninformationen wie Seitenindex und Seitengröße. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Liefert den rechteckigen Bereich. |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | Liefert den Text. |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | Liefert den Textstil wie Schriftgröße, Schriftname und so weiter. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | Konvertiert den Wert dieser Instanz in einen String. |

### Hinweise

Eine Instanz der [`PageTextArea`](../pagetextarea)-Klasse wird als Rückgabewert der folgenden Methoden verwendet:

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

Auch eine Instanz der [`PageTextArea`](../pagetextarea)-Klasse wird als Wert der [`PageArea`](../fielddata/pagearea)-Eigenschaft verwendet.

Siehe dort die Anwendungsbeispiele.

Der Textbereich kann einfach oder zusammengesetzt sein. Im ersten Fall enthält er einen Text, der durch einen rechteckigen Bereich begrenzt ist. Im zweiten Fall enthält er andere Textbereiche; Text- und Tabelleneigenschaften werden von den untergeordneten Textbereichen berechnet.

### Siehe auch

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
