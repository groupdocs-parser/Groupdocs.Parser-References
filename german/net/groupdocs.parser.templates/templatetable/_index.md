---
title: "TemplateTable"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Tabellenvorlage bereit."
type: docs
weight: 160
url: /de/net/groupdocs.parser.templates/templatetable/
---

## TemplateTable class

Stellt die Tabellenvorlage bereit.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string) | Initialisiert eine neue Instanz der [`TemplateTable`](../templatetable)-Klasse mit dem GROSSBUCHSTABEN-Namen. |
| [TemplateTable](templatetable#constructor_3)(TemplateTableParameters, string) | Initialisiert eine neue Instanz der [`TemplateTable`](../templatetable)-Klasse. |
| [TemplateTable](templatetable#constructor_1)(TemplateTableLayout, string, double?) | Initialisiert eine neue Instanz der [`TemplateTable`](../templatetable)-Klasse mit dem GROSSBUCHSTABEN-Namen. |
| [TemplateTable](templatetable#constructor_4)(TemplateTableParameters, string, double?) | Initialisiert eine neue Instanz der [`TemplateTable`](../templatetable)-Klasse. |
| [TemplateTable](templatetable#constructor_2)(TemplateTableLayout, string, double?, bool) | Initialisiert eine neue Instanz der [`TemplateTable`](../templatetable)-Klasse. |
| [TemplateTable](templatetable#constructor_5)(TemplateTableParameters, string, double?, bool) | Initialisiert eine neue Instanz der [`TemplateTable`](../templatetable)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Liefert das Tabellenlayout. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Liefert den Namen des Vorlagen-Elements. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Liefert die Breite der Seite, die zum Erstellen des Vorlagen-Elements verwendet wurde. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Liefert die Parameter, um die Tabelle im automatischen Modus zu erkennen. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Liefert einen booleschen Wert, der angibt, ob ein `Name` in GROSSBUCHSTABEN umgewandelt wurde. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatetable/scale)(double) | Skaliert dieses Vorlagen-Elements um einen angegebenen Faktor. |

### Hinweise

Es gibt zwei Möglichkeiten, eine Tabelle zu definieren:

* Using [`TemplateTableLayout`](../templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [`TemplateTableParameters`](../templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](../templatetableparameters) class for more information.

### Siehe auch

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
