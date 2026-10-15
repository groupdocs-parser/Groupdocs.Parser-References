---
title: "GetHyperlinks"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait les hyperliens du document."
type: docs
weight: 120
url: /fr/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

Extrait les hyperliens du document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Valeur de retour

Une collection d'objets [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ; `null` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire tous les hyperliens du document entier :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction des hyperliens
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
        // Afficher le texte de l'hyperlien
        Console.WriteLine(h.Text);
        // Afficher l'URL de l'hyperlien
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Voir aussi

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extrait les hyperliens de la page du document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une collection d'objets [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ; `null` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les hyperliens de la page du document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction des hyperliens
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Obtenir les informations du document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifier si le document possède des pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Parcourir les pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraire les hyperliens de la page du document
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Itérer sur les hyperliens
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Afficher le texte de l'hyperlien
            Console.WriteLine(h.Text);
            // Afficher l'URL de l'hyperlien
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Voir aussi

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extrait les hyperliens du document en utilisant des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | PageAreaOptions | Les options pour l'extraction des hyperliens. |

### Valeur de retour

Une collection d'objets [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ; `null` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les hyperliens de la zone de la page du document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction des hyperliens
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Créer les options utilisées pour l'extraction des hyperliens
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extraire les hyperliens de la zone de la page du document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Itérer sur les hyperliens
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Afficher le texte de l'hyperlien
        Console.WriteLine(h.Text);
        // Afficher l'URL de l'hyperlien
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Voir aussi

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extrait les hyperliens de la page du document en utilisant des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | PageAreaOptions | Les options pour l'extraction des hyperliens. |

### Valeur de retour

Une collection d'objets [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ; `null` si l'extraction des hyperliens n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les hyperliens de la zone de page du document en utilisant les options de personnalisation :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction des hyperliens
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Obtenir les informations du document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifier si le document possède des pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Créer les options utilisées pour l'extraction des hyperliens
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Parcourir les pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extraire les hyperliens de la zone de la page du document
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Itérer sur les hyperliens
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Afficher le texte de l'hyperlien
            Console.WriteLine(h.Text);
            // Afficher l'URL de l'hyperlien
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Voir aussi

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
