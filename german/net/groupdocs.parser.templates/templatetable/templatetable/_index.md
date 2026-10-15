---
title: "TemplateTable"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Klasse TemplateTablegroupdocs.parser.templates/templatetable mit dem GROSSBUCHSTABEN-Namen."
type: docs
weight: 10
url: /de/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Initialisiert eine neue Instanz der Klasse [`TemplateTable`](../../templatetable) mit dem GROSSBUCHSTABEN-Namen.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| layout | TemplateTableLayout | Das Tabellen-Layout. |
| name | String | Der Tabellenname. |

### Beispiele

Die Vorlagentabelle wird durch das Tabellen-Layout festgelegt, wenn die Tabelle nicht automatisch erkannt werden kann:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Erstelle eine Dokumentvorlage
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Initialisiert eine neue Instanz der Klasse [`TemplateTable`](../../templatetable) mit dem GROSSBUCHSTABEN-Namen.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| layout | TemplateTableLayout | Das Tabellen-Layout. |
| name | String | Der Tabellenname. |
| pageWidth | Nullable`1 | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |

### Beispiele

Die Vorlagentabelle wird durch das Tabellen-Layout festgelegt, wenn die Tabelle nicht automatisch erkannt werden kann:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Erstelle eine Dokumentvorlage
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Initialisiert eine neue Instanz der Klasse [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| layout | TemplateTableLayout | Das Tabellen-Layout. |
| name | String | Der Tabellenname. |
| pageWidth | Nullable`1 | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
| useUpperCaseName | Boolean | Der Wert, der angibt, ob ein `name` in GROSSBUCHSTABEN konvertiert wird. |

### Beispiele

Die Vorlagentabelle wird durch das Tabellen-Layout festgelegt, wenn die Tabelle nicht automatisch erkannt werden kann:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Erstelle eine Dokumentvorlage
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Initialisiert eine neue Instanz der Klasse [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Parameter | TemplateTableParameters | Die Parameter zur Erkennung der Tabelle im automatischen Modus. |
| name | String | Der Tabellenname. |

### Beispiele

Wenn eine Vorlagentabelle durch Detektor-Parameter festgelegt wird, wird die Tabelle automatisch erkannt:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Erstelle eine Dokumentvorlage
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Initialisiert eine neue Instanz der Klasse [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Parameter | TemplateTableParameters | Die Parameter zur Erkennung der Tabelle im automatischen Modus. |
| name | String | Der Tabellenname. |
| pageWidth | Nullable`1 | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |

### Beispiele

Wenn eine Vorlagentabelle durch Detektor-Parameter festgelegt wird, wird die Tabelle automatisch erkannt:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Erstelle eine Dokumentvorlage
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Initialisiert eine neue Instanz der Klasse [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Parameter | TemplateTableParameters | Die Parameter zur Erkennung der Tabelle im automatischen Modus. |
| name | String | Der Tabellenname. |
| pageWidth | Nullable`1 | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
| useUpperCaseName | Boolean | Der Wert, der angibt, ob ein `name` in GROSSBUCHSTABEN konvertiert wird. |

### Beispiele

Wenn eine Vorlagentabelle durch Detektor-Parameter festgelegt wird, wird die Tabelle automatisch erkannt:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Erstelle eine Dokumentvorlage
Template template = new Template(new TemplateItem[] { table });
```

### Siehe auch

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
