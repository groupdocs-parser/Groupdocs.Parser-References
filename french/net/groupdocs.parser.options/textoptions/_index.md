---
title: TextOptions
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Fournit les options utilisées pour lextraction de texte.
type: docs
weight: 580
url: /fr/net/groupdocs.parser.options/textoptions/
---
## TextOptions class

Fournit les options utilisées pour l'extraction de texte.

```csharp
public sealed class TextOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [TextOptions](textoptions)(bool) | Initialise une nouvelle instance du[`TextOptions`](../textoptions) classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; } | Obtient la valeur qui indique si le mode brut est utilisé. |

### Remarques

Une instance de[`TextOptions`](../textoptions) la classe est utilisée comme paramètre dans[`GetText`](../../groupdocs.parser/parser/gettext) et[`GetText`](../../groupdocs.parser/parser/gettext) méthodes. Voir les exemples d'utilisation ici.

Il est utilisé pour spécifier le mode brut d'extraction de texte. Un texte dans ce mode est extrait de manière non précise mais plus rapide qu'en mode standard. Si le mode brut ne prend pas en charge le format du document, alors ce paramètre est ignoré et le mode standard est utilisé.

**Apprendre encore plus:**

* [Extraire du texte en mode précis](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraire du texte en mode brut](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Voir également

* espace de noms [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* Assemblée [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->