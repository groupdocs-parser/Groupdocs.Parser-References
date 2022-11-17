---
title: TemplateTable
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Stellt die Vorlagentabelle bereit.
type: docs
weight: 690
url: /de/net/groupdocs.parser.templates/templatetable/
---
## TemplateTable class

Stellt die Vorlagentabelle bereit.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string, int?) | Initialisiert eine neue Instanz von[`TemplateTable`](../templatetable) Klasse. |
| [TemplateTable](templatetable#constructor_1)(TemplateTableParameters, string, int?) | Initialisiert eine neue Instanz von[`TemplateTable`](../templatetable) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Ruft das Tabellenlayout ab. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Ruft den Namen des Vorlagenelements ab. |
| [PageIndex](../../groupdocs.parser.templates/templateitem/pageindex) { get; } | Ruft den Seitenindex des Vorlagenelements ab. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Ruft die Parameter ab, um die Tabelle im automatischen Modus zu erkennen. |

### Bemerkungen

Es gibt zwei Möglichkeiten, eine Tabelle zu definieren:

* Verwenden[`TemplateTableLayout`](../templatetablelayout) Klasse. In diesem Fall wird die Tabelle durch ihre Position auf der Seite definiert: rechteckige Fläche, Spalten- und Zeilentrennzeichen.
* Verwenden[`TemplateTableParameters`](../templatetableparameters) class. In diesem Fall wird die Tabelle automatisch von Algorithmen mit gesetzten Parametern erkannt. Siehe[`TemplateTableParameters`](../templatetableparameters) Klasse für weitere Informationen.

### Siehe auch

* class [TemplateItem](../templateitem)
* namensraum [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* Montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->