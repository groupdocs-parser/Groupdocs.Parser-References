---
title: PageTextAreaOptions
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Stellt die Optionen bereit die zum Extrahieren von Seitentextbereichen verwendet werden.
type: docs
weight: 500
url: /de/net/groupdocs.parser.options/pagetextareaoptions/
---
## PageTextAreaOptions class

Stellt die Optionen bereit, die zum Extrahieren von Seitentextbereichen verwendet werden.

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)(string) | Initialisiert eine neue Instanz von[`PageTextAreaOptions`](../pagetextareaoptions) Klasse mit dem regulären Ausdruck. Andere Optionen sind standardmäßig eingestellt (siehe Anmerkungen für Details). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(string, Rectangle) | Initialisiert eine neue Instanz von[`PageTextAreaOptions`](../pagetextareaoptions) class mit dem regulären Ausdruck und dem rechteckigen Bereich. Andere Optionen sind standardmäßig eingestellt (siehe Anmerkungen für Details). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(string, bool, bool, bool, Rectangle) | Initialisiert eine neue Instanz von[`PageTextAreaOptions`](../pagetextareaoptions) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; } | Ruft den regulären Ausdruck ab. |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; } | Ruft den Wert ab, der angibt, ob die Textformatierung ignoriert wird. |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; } | Ruft den Wert ab, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; } | Ruft den rechteckigen Bereich ab, der Seitenbereiche enthält. |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; } | Ruft den Wert ab, der angibt, ob Segmente vereint sind. |

### Bemerkungen

Eine Instanz von[`PageTextAreaOptions`](../pagetextareaoptions) Klasse wird als Parameter in verwendet[`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) und[`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) Methoden. Siehe dort die Anwendungsbeispiele. **Mehr erfahren:**

* [Textbereiche extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Siehe auch

* class [PageAreaOptions](../pageareaoptions)
* namensraum [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* Montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->