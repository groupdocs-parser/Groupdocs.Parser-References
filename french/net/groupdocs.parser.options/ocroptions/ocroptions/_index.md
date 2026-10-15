---
title: "OcrOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe OcrOptionsgroupdocs.parser.options/ocroptions avec une zone rectangulaire."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions) avec une zone rectangulaire.

```csharp
public OcrOptions()
```

### Voir aussi

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions) avec une zone rectangulaire.

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | Une instance de la classe [`PagePreviewOptions`](../pagepreviewoptions) qui définit les propriétés pour la génération de l'aperçu de page du document. |

### Voir aussi

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions) avec une zone rectangulaire.

```csharp
public OcrOptions(Rectangle rectangle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rectangle | Rectangle | La zone rectangulaire qui contraint la zone de page utilisée pour la reconnaissance de texte. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions) avec l'objet [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(OcrEventHandler handler)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| handler | OcrEventHandler | Une instance de [`OcrEventHandler`](../../ocreventhandler) pour intercepter les événements OCR. |

### Voir aussi

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions) avec une zone rectangulaire et l'objet [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rectangle | Rectangle | La zone rectangulaire qui contraint la zone de page utilisée pour la reconnaissance de texte. |
| handler | OcrEventHandler | Une instance de [`OcrEventHandler`](../../ocreventhandler) pour intercepter les événements OCR. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rectangle | Rectangle | La zone rectangulaire qui contraint la zone de page utilisée pour la reconnaissance de texte. |
| handler | OcrEventHandler | Une instance de [`OcrEventHandler`](../../ocreventhandler) pour intercepter les événements OCR. |
| pagePreviewOptions | PagePreviewOptions | Une instance de la classe [`PagePreviewOptions`](../pagepreviewoptions) qui définit les propriétés pour la génération de l'aperçu de page du document. |
| useSpellCheker | Booléen | La valeur qui indique si le correcteur orthographique est utilisé. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

Initialise une nouvelle instance de la classe [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rectangle | Rectangle | La zone rectangulaire qui contraint la zone de page utilisée pour la reconnaissance de texte. |
| handler | OcrEventHandler | Une instance de [`OcrEventHandler`](../../ocreventhandler) pour intercepter les événements OCR. |
| pagePreviewOptions | PagePreviewOptions | Une instance de la classe [`PagePreviewOptions`](../pagepreviewoptions) qui définit les propriétés pour la génération de l'aperçu de page du document. |
| useSpellCheker | Booléen | La valeur qui indique si le correcteur orthographique est utilisé. |
| language | Langue | La langue utilisée pour l'OCR. |

### Voir aussi

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
