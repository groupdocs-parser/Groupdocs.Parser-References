---
title: "GetMetadata"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait les métadonnées du document."
type: docs
weight: 140
url: /fr/net/groupdocs.parser/parser/getmetadata/
---

## Parser.GetMetadata method

Extrait les métadonnées du document.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### Valeur de retour

Une collection d'éléments de métadonnées ; `null` si l'extraction de métadonnées n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract metadata from documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Exemples

L'exemple suivant montre comment extraire les métadonnées d'un document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire les métadonnées du document
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // Vérifier si l'extraction des métadonnées est prise en charge
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // Parcourir les éléments de métadonnées
    foreach(MetadataItem item in metadata)
    {
        // Afficher le nom et la valeur d'un élément
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### Voir aussi

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
