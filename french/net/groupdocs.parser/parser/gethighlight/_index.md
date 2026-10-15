---
title: "GetHighlight"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait une mise en évidence du document."
type: docs
weight: 110
url: /fr/net/groupdocs.parser/parser/gethighlight/
---

## Parser.GetHighlight method

Extrait une mise en évidence du document.

```csharp
public HighlightItem GetHighlight(int position, bool isDirect, HighlightOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| position | Int32 | La position de départ du surlignage. |
| isDirect | Booléen | La valeur qui indique si l'extraction du surlignage est directe. `true` si le surlignage est extrait à droite de *position* ; sinon, `false`. |
| options | HighlightOptions | Les options d'extraction du surlignage. |

### Valeur de retour

Une instance de la classe [`HighlightItem`](../../../groupdocs.parser.data/highlightitem) qui représente le surlignage extrait ; `null` si l'extraction du surlignage n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Exemples

L'exemple suivant montre comment extraire un surlignage contenant 3 mots :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire un surlignage :
    HighlightItem hl = parser.GetHighlight(2, true, new HighlightOptions(3));
    
    // Vérifier si l'extraction du surlignage est prise en charge
    if (hl == null)
    {
        Console.WriteLine("Highlight extraction isn't supported");
        return;
    }
    
    // Imprimer un surlignage extrait
    Console.WriteLine(string.Format("At {0}: {1}", hl.Position, hl.Text));
}
```

### Voir aussi

* class [HighlightItem](../../../groupdocs.parser.data/highlightitem)
* class [HighlightOptions](../../../groupdocs.parser.options/highlightoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
