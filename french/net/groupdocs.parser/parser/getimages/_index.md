---
title: GetImages
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait les images du document.
type: docs
weight: 110
url: /fr/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Extrait les images du document.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Return_Value

Une collection de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objets ; `nul` si l'extraction d'images n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des images de documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraire des images dans des fichiers](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraire des images de documents Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraire des images de feuilles de calcul Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraire des images de présentations Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraire des images des e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraire des images de documents PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Exemples

L'exemple suivant montre comment extraire toutes les images de l'ensemble du document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire les images
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Vérifie si l'extraction d'images est supportée
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Itérer sur les images
    foreach (PageImageArea image in images)
    {
        // Impression d'un index de page, rectangle et type d'image :
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Voir également

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Extrait les images du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les images).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | PageAreaOptions | Les options d'extraction d'images. |

### Return_Value

Une collection de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objets ; `nul` si l'extraction d'images n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des images de documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraire des images dans des fichiers](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraire des images de la zone de page du document](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extraire des images de documents Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraire des images de feuilles de calcul Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraire des images de présentations Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraire des images des e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraire des images de documents PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Exemples

L'exemple suivant montre comment extraire uniquement les images du coin supérieur gauche :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Crée les options qui servent à l'extraction des images
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Extrait les images du coin supérieur gauche d'une page :
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Vérifie si l'extraction d'images est supportée
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Itérer sur les images
    foreach (PageImageArea image in images)
    {
        // Impression d'un index de page, rectangle et type d'image :
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Voir également

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Extrait les images de la page du document.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |

### Return_Value

Une collection de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objets ; `nul` si l'extraction d'images n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des images de documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraire des images dans des fichiers](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraire des images de la page du document](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extraire des images de documents Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraire des images de feuilles de calcul Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraire des images de présentations Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraire des images des e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraire des images de documents PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Exemples

Pour extraire des images d'une page de document, la méthode suivante est utilisée :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction d'images
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // Récupère les informations sur le document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifie si le document contient des pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Itérer sur les pages
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Itérer sur les images
        // Nous ignorons la vérification nulle car nous avons vérifié la prise en charge de la fonctionnalité d'extraction d'images plus tôt
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Imprime un rectangle et un type d'image
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Voir également

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Extrait les images de la page du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les images).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | PageAreaOptions | Les options d'extraction d'images. |

### Return_Value

Une collection de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objets ; `nul` si l'extraction d'images n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des images de documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraire des images dans des fichiers](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraire des images de la page du document](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extraire des images de la zone de page du document](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extraire des images de documents Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraire des images de feuilles de calcul Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraire des images de présentations Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraire des images des e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraire des images de documents PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voir également

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
