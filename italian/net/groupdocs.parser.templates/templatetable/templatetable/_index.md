---
title: "TemplateTable"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Inizializza una nuova istanza della classe TemplateTablegroupdocs.parser.templates/templatetable con il nome in MAIUSCOLO."
type: docs
weight: 10
url: /it/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Inizializza una nuova istanza della classe [`TemplateTable`](../../templatetable) con il nome in MAIUSCOLO.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| layout | TemplateTableLayout | Il layout della tabella. |
| nome | Stringa | Il nome della tabella. |

### Esempi

La tabella modello è impostata dal layout della tabella se la tabella non può essere rilevata automaticamente:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Crea un modello di documento
Template template = new Template(new TemplateItem[] { table });
```

### Vedi anche

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Inizializza una nuova istanza della classe [`TemplateTable`](../../templatetable) con il nome in MAIUSCOLO.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| layout | TemplateTableLayout | Il layout della tabella. |
| nome | Stringa | Il nome della tabella. |
| pageWidth | Nullable`1 | La larghezza della pagina che è stata usata per creare l'elemento modello. |

### Esempi

La tabella modello è impostata dal layout della tabella se la tabella non può essere rilevata automaticamente:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Crea un modello di documento
Template template = new Template(new TemplateItem[] { table });
```

### Vedi anche

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Inizializza una nuova istanza della classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| layout | TemplateTableLayout | Il layout della tabella. |
| nome | Stringa | Il nome della tabella. |
| pageWidth | Nullable`1 | La larghezza della pagina che è stata usata per creare l'elemento modello. |
| useUpperCaseName | Boolean | Il valore che indica se un `name` viene convertito in MAIUSCOLE. |

### Esempi

La tabella modello è impostata dal layout della tabella se la tabella non può essere rilevata automaticamente:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Crea un modello di documento
Template template = new Template(new TemplateItem[] { table });
```

### Vedi anche

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Inizializza una nuova istanza della classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| parametri | TemplateTableParameters | I parametri per rilevare la tabella in modalità automatica. |
| nome | Stringa | Il nome della tabella. |

### Esempi

Se una tabella modello è impostata tramite i parametri del rilevatore, la tabella viene rilevata automaticamente:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Crea un modello di documento
Template template = new Template(new TemplateItem[] { table });
```

### Vedi anche

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Inizializza una nuova istanza della classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| parametri | TemplateTableParameters | I parametri per rilevare la tabella in modalità automatica. |
| nome | Stringa | Il nome della tabella. |
| pageWidth | Nullable`1 | La larghezza della pagina che è stata usata per creare l'elemento modello. |

### Esempi

Se una tabella modello è impostata tramite i parametri del rilevatore, la tabella viene rilevata automaticamente:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Crea un modello di documento
Template template = new Template(new TemplateItem[] { table });
```

### Vedi anche

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Inizializza una nuova istanza della classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| parametri | TemplateTableParameters | I parametri per rilevare la tabella in modalità automatica. |
| nome | Stringa | Il nome della tabella. |
| pageWidth | Nullable`1 | La larghezza della pagina che è stata usata per creare l'elemento modello. |
| useUpperCaseName | Boolean | Il valore che indica se un `name` viene convertito in MAIUSCOLE. |

### Esempi

Se una tabella modello è impostata tramite i parametri del rilevatore, la tabella viene rilevata automaticamente:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Crea un modello di documento
Template template = new Template(new TemplateItem[] { table });
```

### Vedi anche

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
