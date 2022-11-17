---
title: TemplateTable
second_title: GroupDocs.Parser för .NET API-referens
description: Tillhandahåller malltabellen.
type: docs
weight: 690
url: /sv/net/groupdocs.parser.templates/templatetable/
---
## TemplateTable class

Tillhandahåller malltabellen.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string, int?) | Initierar en ny instans av[`TemplateTable`](../templatetable) class. |
| [TemplateTable](templatetable#constructor_1)(TemplateTableParameters, string, int?) | Initierar en ny instans av[`TemplateTable`](../templatetable) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Hämtar tabelllayouten. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Hämtar namnet på mallobjektet. |
| [PageIndex](../../groupdocs.parser.templates/templateitem/pageindex) { get; } | Hämtar sidindexet för mallobjektet. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Hämtar parametrarna för att detektera tabellen i automatiskt läge. |

### Anmärkningar

Det finns två sätt att definiera en tabell:

* Använder[`TemplateTableLayout`](../templatetablelayout) klass. I det här fallet definieras tabellen av dess position på sidan: rektangulärt område, kolumner och radavgränsare.
* Använder[`TemplateTableParameters`](../templatetableparameters) class. I detta fall detekteras tabellen automatiskt av algoritmer med inställda parametrar. Se[`TemplateTableParameters`](../templatetableparameters) klass för mer information.

### Se även

* class [TemplateItem](../templateitem)
* namnutrymme [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* hopsättning [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->