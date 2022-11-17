---
title: SearchOptions
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Stellt die Optionen bereit die für die Textsuche verwendet werden.
type: docs
weight: 560
url: /de/net/groupdocs.parser.options/searchoptions/
---
## SearchOptions class

Stellt die Optionen bereit, die für die Textsuche verwendet werden.

```csharp
public sealed class SearchOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | Initialisiert eine neue Instanz von[`SearchOptions`](../searchoptions) Klasse mit Standardwerten. Siehe Bemerkungen für Details. |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | Initialisiert eine neue Instanz von[`SearchOptions`](../searchoptions) Klasse, die verwendet wird, um ohne Highlight-Extraktion zu suchen. |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | Initialisiert eine neue Instanz von[`SearchOptions`](../searchoptions) Klasse, die verwendet wird, um nach Seiten und ohne Highlight-Extraktion zu suchen. |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | Initialisiert eine neue Instanz von[`SearchOptions`](../searchoptions) Klasse, die verwendet wird, um mit denselben Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion zu suchen. |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | Initialisiert eine neue Instanz von[`SearchOptions`](../searchoptions) Klasse, die verwendet wird, um mit den Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion zu suchen. |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | Initialisiert eine neue Instanz von[`SearchOptions`](../searchoptions) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; } | Ruft die Optionen für die linke Markierung ab. |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; } | Ruft den Wert ab, der angibt, ob eine Groß-/Kleinschreibung nicht ignoriert wird. |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; } | Ruft den Wert ab, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; } | Ruft die Optionen für die richtige Hervorhebung ab. |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; } | Ruft den Wert ab, der angibt, ob die Suche seitenweise durchgeführt wird. |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; } | Ruft den Wert ab, der angibt, ob ein regulärer Ausdruck verwendet wird. |

### Bemerkungen

Eine Instanz von[`SearchOptions`](../searchoptions) Klasse wird als Parameter in verwendet[`Search`](../../groupdocs.parser/parser/search) Methode. Siehe dort die Anwendungsbeispiele.

**Mehr erfahren:**

* [Suchtext](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Durchsuchen Sie Text in Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Durchsuchen Sie Text in Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Durchsuchen Sie Text in Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Text in PDF-Dokumenten suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Text in E-Mails suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Suchen Sie Text in EPUB-eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Text in HTML-Dokumenten suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Suchen Sie Text in Microsoft OneNote-Abschnitten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Siehe auch

* namensraum [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* Montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->