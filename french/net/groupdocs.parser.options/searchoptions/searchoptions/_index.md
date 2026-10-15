---
title: "SearchOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| matchWholeWord | Booléen | La valeur qui indique si la recherche de texte est limitée à un mot complet. |
| useRegularExpression | Booléen | La valeur qui indique si une expression régulière est utilisée. |
| searchByPages | Booléen | La valeur qui indique si la recherche est effectuée par pages. |
| leftHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance de gauche. |
| rightHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance de droite. |

### Voir aussi

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions) avec la limite de pages.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| matchWholeWord | Booléen | La valeur qui indique si la recherche de texte est limitée à un mot complet. |
| useRegularExpression | Booléen | La valeur qui indique si une expression régulière est utilisée. |
| maxPageIndex | Int32 | La valeur qui indique si la recherche est effectuée par pages. |
| leftHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance de gauche. |
| rightHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance de droite. |

### Voir aussi

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions) qui est utilisée pour rechercher avec les options de mise en surbrillance pour l'extraction de la mise en surbrillance gauche et droite.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| matchWholeWord | Booléen | La valeur qui indique si la recherche de texte est limitée à un mot complet. |
| useRegularExpression | Booléen | La valeur qui indique si une expression régulière est utilisée. |
| leftHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance de gauche. |
| rightHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance de droite. |

### Voir aussi

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions) qui est utilisée pour rechercher avec les mêmes options de mise en surbrillance pour l'extraction de la mise en surbrillance gauche et droite.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| matchWholeWord | Booléen | La valeur qui indique si la recherche de texte est limitée à un mot complet. |
| useRegularExpression | Booléen | La valeur qui indique si une expression régulière est utilisée. |
| highlightOptions | HighlightOptions | Les options pour les deux mises en surbrillance. |

### Voir aussi

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions) qui est utilisée pour rechercher sans extraction de mise en surbrillance.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| matchWholeWord | Booléen | La valeur qui indique si la recherche de texte est limitée à un mot complet. |
| useRegularExpression | Booléen | La valeur qui indique si une expression régulière est utilisée. |

### Voir aussi

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions) qui est utilisée pour rechercher par pages et sans extraction de mise en surbrillance.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| matchCase | Booléen | La valeur qui indique si la casse du texte n'est pas ignorée. |
| matchWholeWord | Booléen | La valeur qui indique si la recherche de texte est limitée à un mot complet. |
| useRegularExpression | Booléen | La valeur qui indique si une expression régulière est utilisée. |
| searchByPages | Booléen | La valeur qui indique si la recherche est effectuée par pages. |

### Voir aussi

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initialise une nouvelle instance de la classe [`SearchOptions`](../../searchoptions) avec les valeurs par défaut. Voir les remarques pour plus de détails.

```csharp
public SearchOptions()
```

### Remarques

Les propriétés suivantes ont des valeurs par défaut :

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### Voir aussi

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
