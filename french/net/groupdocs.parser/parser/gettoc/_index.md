---
title: "GetToc"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait une table des matières du document."
type: docs
weight: 200
url: /fr/net/groupdocs.parser/parser/gettoc/
---

## Parser.GetToc method

Extrait une table des matières du document.

```csharp
public IEnumerable<TocItem> GetToc()
```

### Valeur de retour

Une collection d'éléments de table des matières ; `null` si l'extraction de la table des matières n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract table of contents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Extract text by table of contents item](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### Exemples

L'exemple suivant montre comment extraire la table des matières d'un fichier CHM :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }

    // Vérifier si l'extraction de la table des matières est prise en charge
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
 
    // Obtenir la table des matières
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // Itérer sur les éléments
    foreach (TocItem i in toc)
    {
        // Imprimer le texte de la table des matières
        Console.WriteLine(i.Text);
        // Vérifier si l'index de page a une valeur
        if (i.PageIndex == null)
        {
            continue;
        }
        // Extraire le texte d'une page
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
