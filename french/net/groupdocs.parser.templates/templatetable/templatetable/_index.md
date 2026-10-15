---
title: "TemplateTable"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe TemplateTablegroupdocs.parser.templates/templatetable avec le nom en MAJUSCULES."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Initialise une nouvelle instance de la classe [`TemplateTable`](../../templatetable) avec le nom en MAJUSCULES.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| layout | TemplateTableLayout | La disposition du tableau. |
| nom | Chaîne | Le nom du tableau. |

### Exemples

Le tableau modèle est défini par la disposition du tableau si le tableau ne peut pas être détecté automatiquement :

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Créer un modèle de document
Template template = new Template(new TemplateItem[] { table });
```

### Voir aussi

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Initialise une nouvelle instance de la classe [`TemplateTable`](../../templatetable) avec le nom en MAJUSCULES.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| layout | TemplateTableLayout | La disposition du tableau. |
| nom | Chaîne | Le nom du tableau. |
| pageWidth | Nullable`1 | La largeur de la page qui a été utilisée pour créer l'élément de modèle. |

### Exemples

Le tableau modèle est défini par la disposition du tableau si le tableau ne peut pas être détecté automatiquement :

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Créer un modèle de document
Template template = new Template(new TemplateItem[] { table });
```

### Voir aussi

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Initialise une nouvelle instance de la classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| layout | TemplateTableLayout | La disposition du tableau. |
| nom | Chaîne | Le nom du tableau. |
| pageWidth | Nullable`1 | La largeur de la page qui a été utilisée pour créer l'élément de modèle. |
| useUpperCaseName | Booléen | La valeur qui indique si un `name` est converti en MAJUSCULE. |

### Exemples

Le tableau modèle est défini par la disposition du tableau si le tableau ne peut pas être détecté automatiquement :

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Créer un modèle de document
Template template = new Template(new TemplateItem[] { table });
```

### Voir aussi

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Initialise une nouvelle instance de la classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paramètres | TemplateTableParameters | Les paramètres pour détecter le tableau en mode automatique. |
| nom | Chaîne | Le nom du tableau. |

### Exemples

Si un tableau modèle est défini par les paramètres du détecteur, le tableau est détecté automatiquement :

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Créer un modèle de document
Template template = new Template(new TemplateItem[] { table });
```

### Voir aussi

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Initialise une nouvelle instance de la classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paramètres | TemplateTableParameters | Les paramètres pour détecter le tableau en mode automatique. |
| nom | Chaîne | Le nom du tableau. |
| pageWidth | Nullable`1 | La largeur de la page qui a été utilisée pour créer l'élément de modèle. |

### Exemples

Si un tableau modèle est défini par les paramètres du détecteur, le tableau est détecté automatiquement :

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Créer un modèle de document
Template template = new Template(new TemplateItem[] { table });
```

### Voir aussi

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Initialise une nouvelle instance de la classe [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paramètres | TemplateTableParameters | Les paramètres pour détecter le tableau en mode automatique. |
| nom | Chaîne | Le nom du tableau. |
| pageWidth | Nullable`1 | La largeur de la page qui a été utilisée pour créer l'élément de modèle. |
| useUpperCaseName | Booléen | La valeur qui indique si un `name` est converti en MAJUSCULE. |

### Exemples

Si un tableau modèle est défini par les paramètres du détecteur, le tableau est détecté automatiquement :

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Créer un modèle de document
Template template = new Template(new TemplateItem[] { table });
```

### Voir aussi

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
