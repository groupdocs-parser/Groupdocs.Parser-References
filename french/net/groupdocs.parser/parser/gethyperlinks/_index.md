---
title: GetHyperlinks
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait les hyperliens du document.
type: docs
weight: 100
url: /fr/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Extrait les hyperliens du document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Return_Value

Une collection de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objets ; `nul` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire tous les liens hypertexte de l'ensemble du document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de lien hypertexte
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extraire les hyperliens du document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Itérer sur les hyperliens
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Imprime le texte du lien hypertexte
        Console.WriteLine(h.Text);
        // Imprimer l'URL du lien hypertexte
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Voir également

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extrait les hyperliens de la page du document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |

### Return_Value

Une collection de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objets ; `nul` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des liens hypertexte de la page du document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de lien hypertexte
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraire les hyperliens de la page du document
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Itérer sur les hyperliens
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Imprime le texte du lien hypertexte
            Console.WriteLine(h.Text);
            // Imprimer l'URL du lien hypertexte
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Voir également

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extrait les hyperliens du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | PageAreaOptions | Les options d'extraction des hyperliens. |

### Return_Value

Une collection de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objets ; `nul` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des liens hypertexte de la zone de page du document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de lien hypertexte
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Crée les options qui sont utilisées pour l'extraction des liens hypertexte
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extraire les hyperliens de la zone de page du document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Itérer sur les hyperliens
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Imprime le texte du lien hypertexte
        Console.WriteLine(h.Text);
        // Imprimer l'URL du lien hypertexte
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Voir également

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extrait les hyperliens de la page du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | PageAreaOptions | Les options d'extraction des hyperliens. |

### Return_Value

Une collection de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objets ; `nul` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des liens hypertexte de la zone de page du document à l'aide des options de personnalisation :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de lien hypertexte
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    
    // Crée les options qui sont utilisées pour l'extraction des liens hypertexte
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Itérer sur les pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extraire les hyperliens de la zone de page du document
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Itérer sur les hyperliens
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Imprime le texte du lien hypertexte
            Console.WriteLine(h.Text);
            // Imprimer l'URL du lien hypertexte
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Voir également

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
