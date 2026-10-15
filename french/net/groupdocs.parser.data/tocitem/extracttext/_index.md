---
title: "ExtractText"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait un texte du document auquel l'objet TocItemgroupdocs.parser.data/tocitem fait référence."
type: docs
weight: 50
url: /fr/net/groupdocs.parser.data/tocitem/extracttext/
---

## TocItem.ExtractText method

Extrait un texte du document auquel l'objet [`TocItem`](../../tocitem) fait référence.

```csharp
public virtual TextReader ExtractText()
```

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait.

### Exemples

L'exemple suivant montre comment extraire un texte à l'aide d'un élément de la table des matières :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // Obtenir la table des matières
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // Vérifier si l'extraction de la table des matières est prise en charge
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // Itérer sur les éléments
    foreach (TocItem tocItem in tocItems)
    {
        // Afficher le texte du chapitre
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [TocItem](../../tocitem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
