---
title: "DetectFileType"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Détecte le type de fichier de l'élément de conteneur."
type: docs
weight: 60
url: /fr/net/groupdocs.parser.data/containeritem/detectfiletype/
---

## ContainerItem.DetectFileType method

Détecte le type de fichier de l'élément de conteneur.

```csharp
public FileType DetectFileType(FileTypeDetectionMode detectionMode)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| detectionMode | FileTypeDetectionMode | Définit un mode de détection du type de fichier. |

### Valeur de retour

Une instance de la classe [`FileType`](../../../groupdocs.parser.options/filetype) ; [`Unknown`](../../../groupdocs.parser.options/filetype/unknown) si le type de fichier n'est pas détecté.

### Remarques

*detectionMode* parameter provides the ability to control file type detection:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

### Exemples

L'exemple suivant montre comment détecter le type de fichier d'un élément de conteneur :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire les pièces jointes du conteneur
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Vérifier si l'extraction du conteneur est prise en charge
    if (attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
    // Parcourir les pièces jointes
    foreach (ContainerItem item in attachments)
    {
        // Détecter le type de fichier
        Options.FileType fileType = item.DetectFileType(Options.FileTypeDetectionMode.Default);

        // Afficher le nom et le type de fichier
        Console.WriteLine(string.Format("{0}: {1}", item.Name, fileType));
    }
}
```

### Voir aussi

* class [FileType](../../../groupdocs.parser.options/filetype)
* enum [FileTypeDetectionMode](../../../groupdocs.parser.options/filetypedetectionmode)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
