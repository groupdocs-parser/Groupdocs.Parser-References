---
title: "GetFormattedText"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait un texte formaté du document."
type: docs
weight: 100
url: /fr/net/groupdocs.parser/parser/getformattedtext/
---

## GetFormattedText(FormattedTextOptions) {#getformattedtext}

Extrait un texte formaté du document.

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | FormattedTextOptions | Les options d'extraction du texte formaté. |

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait ; `null` si l'extraction de texte formaté n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Exemples

L'exemple suivant montre comment extraire le texte d'un document au format HTML :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire un texte formaté dans le lecteur
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // Afficher un texte formaté depuis le document
        // Si l'extraction de texte formaté n'est pas prise en charge, le lecteur est `null`
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### Voir aussi

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

Extrait un texte formaté de la page du document.

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | FormattedTextOptions | Les options d'extraction du texte formaté. |

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait ; `null` si l'extraction de texte formaté de page n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Exemples

L'exemple suivant montre comment extraire le texte d'une page de document au format Markdown :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de texte formaté
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
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
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // Extraire un texte formaté dans le lecteur
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // Afficher un texte formaté depuis le document
            // Nous ignorons la vérification de null car nous avons déjà vérifié le support de la fonctionnalité d'extraction de texte formaté
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
