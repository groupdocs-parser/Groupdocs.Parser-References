---
title: GetTextAreas
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait des zones de texte du document.
type: docs
weight: 160
url: /fr/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Extrait des zones de texte du document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Return_Value

Une collection de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objets ; `nul` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des zones de texte](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exemples

L'exemple suivant montre comment extraire toutes les zones de texte de l'ensemble du document :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraction des zones de texte
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Vérifie si l'extraction des zones de texte est supportée
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itérer sur les zones de texte de la page
    foreach(PageTextArea a in areas)
    {
        // Affiche une valeur d'index de page, de rectangle et de zone de texte :
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Voir également

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extrait des zones de texte du document à l'aide d'options de personnalisation (expression régulière, correspondance de casse, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | PageTextAreaOptions | Les options d'extraction de zone de texte. |

### Return_Value

Une collection de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objets ; `nul` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des zones de texte](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exemples

L'exemple suivant montre comment extraire uniquement les zones de texte avec des chiffres du coin supérieur gauche :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Crée les options qui sont utilisées pour l'extraction de la zone de texte
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extrait les zones de texte qui ne contiennent que des chiffres du coin supérieur gauche d'une page :
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Vérifie si l'extraction des zones de texte est supportée
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itérer sur les zones de texte de la page
    foreach(PageTextArea a in areas)
    {
        // Affiche une valeur d'index de page, de rectangle et de zone de texte :
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Voir également

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extrait les zones de texte de la page du document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |

### Return_Value

Une collection de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objets ; `nul` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des zones de texte](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exemples

Pour extraire des zones de texte d'une page de document, la méthode suivante est utilisée :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction des zones de texte
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Récupère les informations sur le document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifie si le document contient des pages
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itérer sur les pages
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Itérer sur les zones de texte de la page
        // Nous ignorons la vérification des valeurs nulles car nous avons vérifié précédemment la prise en charge de la fonction d'extraction des zones de texte
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Affiche un rectangle et une valeur de zone de texte :
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Voir également

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extrait des zones de texte de la page du document à l'aide d'options de personnalisation (expression régulière, correspondance de casse, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | PageTextAreaOptions | Les options d'extraction de zone de texte. |

### Return_Value

Une collection de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objets ; `nul` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire des zones de texte](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voir également

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
