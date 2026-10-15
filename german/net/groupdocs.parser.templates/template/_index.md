---
title: "Template"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Dokumentenseiten‑Vorlage bereit. Sie besteht aus TemplateItem./templateitem‑Objekten, die die Elemente der Vorlage wie Textfelder und Tabellendefinitionen darstellen."
type: docs
weight: 50
url: /de/net/groupdocs.parser.templates/template/
---

## Template class

Stellt die Dokumentenseiten‑Vorlage bereit. Sie besteht aus [`TemplateItem`](../templateitem)-Objekten, die die Elemente der Vorlage wie Textfelder und Tabellendefinitionen darstellen.

```csharp
public sealed class Template : IEnumerable<TemplateItem>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Template](template#constructor)(IEnumerable&lt;TemplateItem&gt;) | Initialisiert eine neue Instanz der [`Template`](../template)-Klasse. |
| [Template](template#constructor_1)(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) | Initialisiert eine neue Instanz der [`Template`](../template)-Klasse mit Vorlagenoptionen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.parser.templates/template/count) { get; } | Gibt die Gesamtzahl der Vorlagen‑Elemente zurück. |
| [IsOcrCompatible](../../groupdocs.parser.templates/template/isocrcompatible) { get; } | Ermittelt den Wert, der angibt, ob die Vorlage mit OCR kompatibel ist. |
| [Item](../../groupdocs.parser.templates/template/item) { get; } | Ermittelt das Vorlagen-Element über einen Index. |
| [Options](../../groupdocs.parser.templates/template/options) { get; } | Ermittelt die Vorlagenoptionen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Load](../../groupdocs.parser.templates/template/load#load)(Stream) | Lädt eine Vorlage aus einem Stream. |
| static [Load](../../groupdocs.parser.templates/template/load#load_1)(string) | Lädt eine Vorlage aus einer Datei. |
| [GetEnumerator](../../groupdocs.parser.templates/template/getenumerator)() | Gibt einen Enumerator für Vorlagen-Elemente zurück. |
| [Save](../../groupdocs.parser.templates/template/save#save)(Stream) | Speichert eine Vorlage in einen Stream. |
| [Save](../../groupdocs.parser.templates/template/save#save_1)(string) | Speichert eine Vorlage in einer Datei. |

### Hinweise

**Learn more:**

* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)

### Siehe auch

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
