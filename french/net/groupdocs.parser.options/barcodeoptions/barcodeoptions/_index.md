---
title: "BarcodeOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe BarcodeOptionsgroupdocs.parser.options/barcodeoptions avec les valeurs par défaut."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/barcodeoptions/barcodeoptions/
---

## BarcodeOptions() {#constructor}

Initialise une nouvelle instance de la classe [`BarcodeOptions`](../../barcodeoptions) avec les valeurs par défaut.

```csharp
public BarcodeOptions()
```

### Voir aussi

* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle) {#constructor_1}

Initialise une nouvelle instance de la classe [`BarcodeOptions`](../../barcodeoptions) avec la zone rectangulaire.

```csharp
public BarcodeOptions(Rectangle rectangle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rectangle | Rectangle | La zone rectangulaire qui contient les codes-barres. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(QualityMode, QualityMode, params string[]) {#constructor_3}

Initialise une nouvelle instance de la classe [`BarcodeOptions`](../../barcodeoptions) avec des paramètres de qualité et des types de code.

```csharp
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, 
    params string[] codeTypes)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageQuality | QualityMode | La qualité d'une image source. |
| barcodeQuality | QualityMode | La qualité d'un code-barres source. |
| codeTypes | String[] | Les types de codes-barres à lire. |

### Voir aussi

* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) {#constructor_2}

Initialise une nouvelle instance de la classe [`BarcodeOptions`](../../barcodeoptions).

```csharp
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, 
    float? dimension, bool allowIncorrectBarcodes, params string[] codeTypes)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rectangle | Rectangle | La zone rectangulaire qui contient les codes-barres. |
| imageQuality | QualityMode | La qualité d'une image source. |
| barcodeQuality | QualityMode | La qualité d'un code-barres source. |
| dimension | Nullable`1 | La taille minimale de l'élément minimal du code-barres. |
| allowIncorrectBarcodes | Booléen | La valeur qui indique si les codes-barres incorrects sont autorisés. |
| codeTypes | String[] | Les types de codes-barres à lire. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
