---
title: "SearchOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für die Textsuche verwendet werden."
type: docs
weight: 590
url: /de/net/groupdocs.parser.options/searchoptions/
---

## SearchOptions class

Stellt die Optionen bereit, die für die Textsuche verwendet werden.

```csharp
public sealed class SearchOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse mit Standardwerten. Siehe Anmerkungen für Details. |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse, die zum Suchen ohne Hervorhebungs-Extraktion verwendet wird. |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse, die zum Suchen nach Seiten und ohne Hervorhebungs-Extraktion verwendet wird. |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse, die zum Suchen mit denselben Hervorhebungsoptionen für die linke und rechte Hervorhebungs-Extraktion verwendet wird. |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse, die zum Suchen mit den Hervorhebungsoptionen für die linke und rechte Hervorhebungs-Extraktion verwendet wird. |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse. |
| [SearchOptions](searchoptions#constructor_6)(bool, bool, bool, int, HighlightOptions, HighlightOptions) | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse mit dem Seitenlimit. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; set; } | Ruft die Optionen für die linke Hervorhebung ab. |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; set; } | Ermittelt den Wert, der angibt, ob die Groß-/Kleinschreibung des Textes nicht ignoriert wird. |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; set; } | Ruft den Wert ab, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
| [MaxPageIndex](../../groupdocs.parser.options/searchoptions/maxpageindex) { get; set; } | Ruft den Wert ab, der den maximalen Index der zu durchsuchenden Seite darstellt. |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; set; } | Ruft die Optionen für die rechte Hervorhebung ab. |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; set; } | Ruft den Wert ab, der angibt, ob die Suche seitenweise durchgeführt wird. |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; set; } | Ruft den Wert ab, der angibt, ob ein regulärer Ausdruck verwendet wird. |

### Hinweise

Eine Instanz der [`SearchOptions`](../searchoptions)-Klasse wird als Parameter in der [`Search`](../../groupdocs.parser/parser/search)-Methode verwendet. Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
