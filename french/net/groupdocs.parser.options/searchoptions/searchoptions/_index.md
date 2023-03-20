---
title: SearchOptions
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Initialise une nouvelle instance duSearchOptionsgroupdocs.parser.options/searchoptions classe.
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initialise une nouvelle instance du[`SearchOptions`](../../searchoptions) classe.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| matchCase | Boolean | La valeur qui indique si une casse de texte n'est pas ignorée. |
| matchWholeWord | Boolean | La valeur qui indique si la recherche de texte est limitée par un mot entier. |
| useRegularExpression | Boolean | La valeur qui indique si une expression régulière est utilisée. |
| searchByPages | Boolean | La valeur qui indique si la recherche est effectuée par pages. |
| leftHighlightOptions | HighlightOptions | Les options pour la surbrillance gauche. |
| rightHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance droite. |

### Voir également

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* espace de noms [GroupDocs.Parser.Options](../../searchoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initialise une nouvelle instance du[`SearchOptions`](../../searchoptions) classe qui est utilisée pour rechercher avec les options de surbrillance pour l'extraction de surbrillance gauche et droite.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| matchCase | Boolean | La valeur qui indique si une casse de texte n'est pas ignorée. |
| matchWholeWord | Boolean | La valeur qui indique si la recherche de texte est limitée par un mot entier. |
| useRegularExpression | Boolean | La valeur qui indique si une expression régulière est utilisée. |
| leftHighlightOptions | HighlightOptions | Les options pour la surbrillance gauche. |
| rightHighlightOptions | HighlightOptions | Les options pour la mise en surbrillance droite. |

### Voir également

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* espace de noms [GroupDocs.Parser.Options](../../searchoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initialise une nouvelle instance du[`SearchOptions`](../../searchoptions) classe qui est utilisée pour rechercher avec les mêmes options de surbrillance pour l'extraction de surbrillance gauche et droite.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| matchCase | Boolean | La valeur qui indique si une casse de texte n'est pas ignorée. |
| matchWholeWord | Boolean | La valeur qui indique si la recherche de texte est limitée par un mot entier. |
| useRegularExpression | Boolean | La valeur qui indique si une expression régulière est utilisée. |
| highlightOptions | HighlightOptions | Les options pour les deux faits saillants. |

### Voir également

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* espace de noms [GroupDocs.Parser.Options](../../searchoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initialise une nouvelle instance du[`SearchOptions`](../../searchoptions) classe qui est utilisée pour rechercher sans extraction de surbrillance.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| matchCase | Boolean | La valeur qui indique si une casse de texte n'est pas ignorée. |
| matchWholeWord | Boolean | La valeur qui indique si la recherche de texte est limitée par un mot entier. |
| useRegularExpression | Boolean | La valeur qui indique si une expression régulière est utilisée. |

### Voir également

* class [SearchOptions](../../searchoptions)
* espace de noms [GroupDocs.Parser.Options](../../searchoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initialise une nouvelle instance du[`SearchOptions`](../../searchoptions)classe qui est utilisée pour rechercher par pages et sans extraction de surbrillance.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| matchCase | Boolean | La valeur qui indique si une casse de texte n'est pas ignorée. |
| matchWholeWord | Boolean | La valeur qui indique si la recherche de texte est limitée par un mot entier. |
| useRegularExpression | Boolean | La valeur qui indique si une expression régulière est utilisée. |
| searchByPages | Boolean | La valeur qui indique si la recherche est effectuée par pages. |

### Voir également

* class [SearchOptions](../../searchoptions)
* espace de noms [GroupDocs.Parser.Options](../../searchoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initialise une nouvelle instance du[`SearchOptions`](../../searchoptions) classe avec des valeurs par défaut. Voir les remarques pour plus de détails.

```csharp
public SearchOptions()
```

### Remarques

Les propriétés suivantes ont des valeurs par défaut :

**[`MatchCase`](../matchcase)**

`FAUX`

**[`MatchWholeWord`](../matchwholeword)**

`FAUX`

**[`UseRegularExpression`](../useregularexpression)**

`FAUX`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`nul`

**[`RightHighlightOptions`](../righthighlightoptions)**

`nul`

### Voir également

* class [SearchOptions](../../searchoptions)
* espace de noms [GroupDocs.Parser.Options](../../searchoptions)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
