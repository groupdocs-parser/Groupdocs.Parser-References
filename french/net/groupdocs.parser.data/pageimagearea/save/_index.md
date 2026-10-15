---
title: "Enregistrer"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Enregistre l'image dans le fichier."
type: docs
weight: 50
url: /fr/net/groupdocs.parser.data/pageimagearea/save/
---

## Save(string) {#save}

Enregistre l'image dans le fichier.

```csharp
public void Save(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |

### Exemples

L'exemple suivant montre comment enregistrer des images dans des fichiers:

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire des images du document
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Vérifier si l'extraction d'images est prise en charge
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Parcourir les images
    foreach (PageImageArea image in images)
    {
        // Enregistrer l'image dans le fichier
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### Voir aussi

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

Enregistre l'image dans le fichier dans un format différent.

```csharp
public void Save(string filePath, ImageOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |
| options | ImageOptions | Les options utilisées pour enregistrer l'image. |

### Exemples

L'exemple suivant montre comment enregistrer des images dans des fichiers dans un format différent :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire des images du document
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Vérifier si l'extraction d'images est prise en charge
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Créer les options pour enregistrer les images au format PNG
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // Parcourir les images
    foreach (PageImageArea image in images)
    {
        // Enregistrer l'image dans le fichier png
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### Voir aussi

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
