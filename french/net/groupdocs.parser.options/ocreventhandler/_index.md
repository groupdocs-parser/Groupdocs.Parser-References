---
title: "OcrEventHandler"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit un gestionnaire pour les événements OCR."
type: docs
weight: 440
url: /fr/net/groupdocs.parser.options/ocreventhandler/
---

## OcrEventHandler class

Fournit un gestionnaire pour les événements OCR.

```csharp
public class OcrEventHandler
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OcrEventHandler](ocreventhandler)() | Initialise une nouvelle instance de la classe [`OcrEventHandler`](../ocreventhandler). |

## Propriétés

| Nom | Description |
| --- | --- |
| [HasWarnings](../../groupdocs.parser.options/ocreventhandler/haswarnings) { get; } | Obtient la valeur qui indique si la liste d'avertissements n'est pas vide. |
| [Warnings](../../groupdocs.parser.options/ocreventhandler/warnings) { get; } | Obtient une liste de messages d'avertissement. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetWarnings](../../groupdocs.parser.options/ocreventhandler/getwarnings)(int) | Renvoie une liste de messages d'avertissement pour la page avec *pageIndex*. |
| virtual [OnWarnings](../../groupdocs.parser.options/ocreventhandler/onwarnings)(int, IList&lt;string&gt;) | Définit les messages d'avertissement pour la page. |

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
