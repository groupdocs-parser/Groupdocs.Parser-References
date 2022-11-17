---
title: TemplateTable
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Initialisiert eine neue Instanz vonTemplateTablegroupdocs.parser.templates/templatetable Klasse.
type: docs
weight: 10
url: /de/net/groupdocs.parser.templates/templatetable/templatetable/
---
## TemplateTable(TemplateTableLayout, string, int?) {#constructor}

Initialisiert eine neue Instanz von[`TemplateTable`](../../templatetable) Klasse.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, int? pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| layout | TemplateTableLayout | Das Tabellenlayout. |
| name | String | Der Tabellenname. |
| pageIndex | Nullable`1 | Der Index der Seite, auf der sich die Vorlagentabelle befindet; `Null` wenn sich die Vorlagentabelle auf einer beliebigen Seite befindet. |

### Beispiele

Die Vorlagentabelle wird vom Tabellenlayout festgelegt, wenn die Tabelle nicht automatisch erkannt werden kann:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Dokumentvorlage erstellen
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namensraum [GroupDocs.Parser.Templates](../../templatetable)
* Montage [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, int?) {#constructor_1}

Initialisiert eine neue Instanz von[`TemplateTable`](../../templatetable) Klasse.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, int? pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| parameters | TemplateTableParameters | Die Parameter zur Erkennung der Tabelle im automatischen Modus. |
| name | String | Der Tabellenname. |
| pageIndex | Nullable`1 | Der Index der Seite, auf der sich die Vorlagentabelle befindet; `Null` wenn sich die Vorlagentabelle auf einer beliebigen Seite befindet. |

### Beispiele

Wenn eine Vorlagentabelle durch Detektorparameter festgelegt wird, wird die Tabelle automatisch erkannt:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Dokumentvorlage erstellen
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namensraum [GroupDocs.Parser.Templates](../../templatetable)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->