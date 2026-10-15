---
title: "GetTextAreas"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait les zones de texte du document."
type: docs
weight: 190
url: /fr/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

Extrait les zones de texte du document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Valeur de retour

Une collection d'objets [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ; `null` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exemples

L'exemple suivant montre comment extraire toutes les zones de texte du document entier :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire les zones de texte
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Vérifier si l'extraction des zones de texte est prise en charge
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Parcourir les zones de texte de la page
    foreach(PageTextArea a in areas)
    {
        // Afficher un index de page, le rectangle et la valeur de la zone de texte :
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extrait les zones de texte du document en utilisant des options de personnalisation (expression régulière, respect de la casse, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | PageTextAreaOptions | Les options pour l'extraction des zones de texte. |

### Valeur de retour

Une collection d'objets [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ; `null` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exemples

L'exemple suivant montre comment extraire uniquement les zones de texte contenant des chiffres depuis le coin supérieur gauche :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Créer les options utilisées pour l'extraction des zones de texte
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extraire les zones de texte qui ne contiennent que des chiffres depuis le coin supérieur gauche d'une page :
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Vérifier si l'extraction des zones de texte est prise en charge
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Parcourir les zones de texte de la page
    foreach(PageTextArea a in areas)
    {
        // Afficher un index de page, le rectangle et la valeur de la zone de texte :
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extrait les zones de texte de la page du document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une collection d'objets [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ; `null` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exemples

Pour extraire les zones de texte d'une page de document, la méthode suivante est utilisée :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction des zones de texte
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Obtenir les informations du document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifier si le document possède des pages
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Parcourir les pages
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Parcourir les zones de texte de la page
        // Nous ignorons la vérification de null car nous avons déjà vérifié le support de la fonctionnalité d'extraction des zones de texte
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Afficher un rectangle et la valeur de la zone de texte :
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extrait les zones de texte de la page du document en utilisant des options de personnalisation (expression régulière, respect de la casse, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | PageTextAreaOptions | Les options pour l'extraction des zones de texte. |

### Valeur de retour

Une collection d'objets [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ; `null` si l'extraction des zones de texte n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
