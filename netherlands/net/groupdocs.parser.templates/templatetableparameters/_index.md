---
title: TemplateTableParameters
second_title: GroupDocs.Parser voor .NET API-referentie
description: Biedt parameters voor de algoritmen voor tabeldetectie.
type: docs
weight: 760
url: /nl/net/groupdocs.parser.templates/templatetableparameters/
---
## TemplateTableParameters class

Biedt parameters voor de algoritmen voor tabeldetectie.

```csharp
public sealed class TemplateTableParameters
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Initialiseert een nieuw exemplaar van het[`TemplateTableParameters`](../templatetableparameters) klasse. |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Initialiseert een nieuw exemplaar van het[`TemplateTableParameters`](../templatetableparameters) klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Haalt de waarde op die aangeeft of de tabel samengevoegde cellen heeft. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Haalt het minimum aantal tabelkolommen op. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Haalt het minimum aantal tabelrijen op. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Haalt de minimale ruimte tussen de tabelkolommen op. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Haalt het rechthoekige gebied op dat de tabel bevat. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Haalt de scheidingstekens van de tabelkolommen op. |

### Opmerkingen

Er zijn twee algoritmen om een tabel te detecteren:

* Maakt het mogelijk een tabel te detecteren in het rechthoekige gebied met vaste kolommen. Dit algoritme is handig voor eenvoudige tabellen (zonder samengevoegde kolommen) en zorgt voor een nauwkeurigere detectie.
* Hiermee kan een tabel op elke plaats op de pagina worden gedetecteerd. Dit is een complexer algoritme. Het kan tabellen op elke plaats op de pagina detecteren. Aanvullende parameters helpen om een tabel correcter te detecteren.

In sommige gevallen wanneer algoritmen een tabel niet kunnen detecteren of dit op een niet-nauwkeurige manier doen [`TemplateTableLayout`](../templatetablelayout) klasse wordt gebruikt.

### Zie ook

* naamruimte [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->