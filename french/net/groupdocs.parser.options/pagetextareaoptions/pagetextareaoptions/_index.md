---
title: "PageTextAreaOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions avec l'option d'utilisation de l'OCR."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec l'option d'utilisation de l'OCR.

```csharp
public PageTextAreaOptions()
```

### Voir aussi

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec l'option d'utilisation de l'OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| useOcr | Booléen | La valeur qui indique si la fonctionnalité OCR est utilisée pour extraire les zones de texte. |

### Voir aussi

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec la possibilité de définir les options OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| useOcr | Booléen | La valeur qui indique si la fonctionnalité OCR est utilisée pour extraire les zones de texte. |
| ocrOptions | OcrOptions | Les options supplémentaires pour la fonctionnalité OCR. |

### Voir aussi

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec l'expression régulière. Les autres options sont définies par défaut (voir les remarques pour plus de détails).

```csharp
public PageTextAreaOptions(string expression)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| expression | Chaîne | L'expression régulière. |

### Remarques

Les propriétés suivantes ont des valeurs par défaut :

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### Voir aussi

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec l'expression régulière et la zone rectangulaire. Les autres options sont définies par défaut (voir les remarques pour plus de détails).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| expression | Chaîne | L'expression régulière. |
| rectangle | Rectangle | La zone rectangulaire qui contient les zones de page. |

### Remarques

Les propriétés suivantes ont des valeurs par défaut :

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec l'expression régulière, la zone rectangulaire et la taille de la bordure ignorée. Les autres options sont définies par défaut (voir les remarques pour plus de détails).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| expression | Chaîne | L'expression régulière. |
| rectangle | Rectangle | La zone rectangulaire qui contient les zones de page. |
| rectangleTolerance | Double | La taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions).

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| expression | Chaîne | L'expression régulière. |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| uniteSegments | Booléen | La valeur qui indique si les segments sont unis. |
| ignoreFormatting | Booléen | La valeur qui indique si le formatage du texte est ignoré. |
| rectangle | Rectangle | La zone rectangulaire qui contient les zones de page. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../../pagetextareaoptions) avec la taille de la bordure ignorée.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| expression | Chaîne | L'expression régulière. |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| uniteSegments | Booléen | La valeur qui indique si les segments sont unis. |
| ignoreFormatting | Booléen | La valeur qui indique si le formatage du texte est ignoré. |
| rectangle | Rectangle | La zone rectangulaire qui contient les zones de page. |
| rectangleTolerance | Double | La taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
