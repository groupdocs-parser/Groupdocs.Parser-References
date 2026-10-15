---
title: "GetImageStream"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Renvoie le flux d'image."
type: docs
weight: 40
url: /fr/net/groupdocs.parser.data/pageimagearea/getimagestream/
---

## GetImageStream() {#getimagestream}

Renvoie le flux d'image.

```csharp
public Stream GetImageStream()
```

### Valeur de retour

Un flux contenant l'image.

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
        // Ouvrir le flux d'image
        using (Stream imageStream = image.GetImageStream())
        {
            // Créer le fichier pour enregistrer l'image
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Lire les données du flux d'image
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Écrire les données dans le flux du fichier
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Voir aussi

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

Renvoie le flux d'image dans un format différent.

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | ImageOptions | Les options utilisées pour extraire l'image. |

### Valeur de retour

Un flux contenant l'image.

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
        // Ouvrir le flux d'image
        using (Stream imageStream = image.GetImageStream(options))
        {
            // Créer le fichier pour enregistrer l'image
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Lire les données du flux d'image
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Écrire les données dans le flux du fichier
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Voir aussi

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
