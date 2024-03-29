---
title: TemplateFixedPosition
second_title: GroupDocs.Parser voor .NET API-referentie
description: Biedt een sjabloonveldpositie die wordt gedefinieerd door het rechthoekige gebied.
type: docs
weight: 680
url: /nl/net/groupdocs.parser.templates/templatefixedposition/
---
## TemplateFixedPosition class

Biedt een sjabloonveldpositie die wordt gedefinieerd door het rechthoekige gebied.

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | Initialiseert een nieuw exemplaar van het[`TemplateFixedPosition`](../templatefixedposition) klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | Haalt het rechthoekige gebied op dat het sjabloonveld bevat. |

### Voorbeelden

Dit is de eenvoudigste manier om de veldpositie te definiëren. Hiervoor moet een rechthoekig gebied op de pagina worden ingesteld dat de veldwaarde begrenst. Alle tekst die (zelfs gedeeltelijk) in het rechthoekige gebied staat, wordt als een waarde geëxtraheerd:

```csharp
// Maak een vast sjabloonveld met de naam "Adres" dat wordt begrensd door een rechthoek op de positie (35, 160) en met de grootte (110, 20)
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### Zie ook

* class [TemplatePosition](../templateposition)
* naamruimte [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
