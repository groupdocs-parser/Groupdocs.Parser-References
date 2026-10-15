---
title: "TemplateTable"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Initialiseert een nieuwe instantie van de TemplateTablegroupdocs.parser.templates/templatetable klasse met de naam in HOOFDLETTERS."
type: docs
weight: 10
url: /nl/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Initialiseert een nieuwe instantie van de [`TemplateTable`](../../templatetable) klasse met de naam in HOOFDLETTERS.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| layout | TemplateTableLayout | De tabelindeling. |
| name | String | De tabelnaam. |

### Voorbeelden

Sjabloontabel wordt ingesteld door de tabelindeling als de tabel niet automatisch kan worden gedetecteerd:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Maak een documentsjabloon
Template template = new Template(new TemplateItem[] { table });
```

### Zie ook

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Initialiseert een nieuwe instantie van de [`TemplateTable`](../../templatetable) klasse met de naam in HOOFDLETTERS.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| layout | TemplateTableLayout | De tabelindeling. |
| name | String | De tabelnaam. |
| pageWidth | Nullable`1 | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |

### Voorbeelden

Sjabloontabel wordt ingesteld door de tabelindeling als de tabel niet automatisch kan worden gedetecteerd:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Maak een documentsjabloon
Template template = new Template(new TemplateItem[] { table });
```

### Zie ook

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`TemplateTable`](../../templatetable) klasse.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| layout | TemplateTableLayout | De tabelindeling. |
| name | String | De tabelnaam. |
| pageWidth | Nullable`1 | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
| useUpperCaseName | Boolean | De waarde die aangeeft of een `name` wordt omgezet naar HOOFDLETTERS. |

### Voorbeelden

Sjabloontabel wordt ingesteld door de tabelindeling als de tabel niet automatisch kan worden gedetecteerd:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Maak een documentsjabloon
Template template = new Template(new TemplateItem[] { table });
```

### Zie ook

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`TemplateTable`](../../templatetable) klasse.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| parameters | TemplateTableParameters | De parameters om de tabel in de automatische modus te detecteren. |
| name | String | De tabelnaam. |

### Voorbeelden

Als een sjabloontabel is ingesteld door detectorparameters, wordt de tabel automatisch gedetecteerd:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Maak een documentsjabloon
Template template = new Template(new TemplateItem[] { table });
```

### Zie ook

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Initialiseert een nieuw exemplaar van de [`TemplateTable`](../../templatetable) klasse.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| parameters | TemplateTableParameters | De parameters om de tabel in de automatische modus te detecteren. |
| name | String | De tabelnaam. |
| pageWidth | Nullable`1 | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |

### Voorbeelden

Als een sjabloontabel is ingesteld door detectorparameters, wordt de tabel automatisch gedetecteerd:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Maak een documentsjabloon
Template template = new Template(new TemplateItem[] { table });
```

### Zie ook

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Initialiseert een nieuw exemplaar van de [`TemplateTable`](../../templatetable) klasse.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| parameters | TemplateTableParameters | De parameters om de tabel in de automatische modus te detecteren. |
| name | String | De tabelnaam. |
| pageWidth | Nullable`1 | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
| useUpperCaseName | Boolean | De waarde die aangeeft of een `name` wordt omgezet naar HOOFDLETTERS. |

### Voorbeelden

Als een sjabloontabel is ingesteld door detectorparameters, wordt de tabel automatisch gedetecteerd:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Maak een documentsjabloon
Template template = new Template(new TemplateItem[] { table });
```

### Zie ook

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
