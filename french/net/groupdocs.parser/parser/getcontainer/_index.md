---
title: "GetContainer"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait un objet conteneur du document pour travailler avec les formats qui contiennent des pièces jointes, des archives ZIP, etc."
type: docs
weight: 80
url: /fr/net/groupdocs.parser/parser/getcontainer/
---

## Parser.GetContainer method

Extrait un objet conteneur du document pour travailler avec des formats contenant des pièces jointes, des archives ZIP, etc.

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### Valeur de retour

Une collection d'éléments de conteneur ; `null` si l'extraction du conteneur n'est pas prise en charge.

### Remarques

Pour vérifier si le format prend en charge l'extraction des pièces jointes, consultez [Supported Document Formats](https://docs.groupdocs.com/parser/net/supported-document-formats/) (colonne **Extract Containers and Attachments**).

**Learn more:**

* [Extract data from attachments and ZIP archives](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### Exemples

L'exemple suivant montre comment extraire les pièces jointes d'un conteneur :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire les pièces jointes du conteneur
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Vérifier si l'extraction du conteneur est prise en charge
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // Parcourir les pièces jointes
    foreach(ContainerItem item in attachments)
    {
        // Imprimer le nom et la taille d'un élément
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### Voir aussi

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
