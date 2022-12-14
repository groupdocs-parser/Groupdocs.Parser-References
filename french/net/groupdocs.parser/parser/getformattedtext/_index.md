---
title: GetFormattedText
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait un texte formaté du document.
type: docs
weight: 80
url: /fr/net/groupdocs.parser/parser/getformattedtext/
---
## GetFormattedText(FormattedTextOptions) {#getformattedtext}

Extrait un texte formaté du document.

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | FormattedTextOptions | Les options d'extraction de texte formaté. |

### Return_Value

Une instance deTextReader classe avec le texte extrait ; `nul` si l'extraction de texte formaté n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire le texte formaté du document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extraire un texte de document comme[HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extraire un texte de document comme[Réduction](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extraire un texte de document comme[Texte brut](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Exemples

L'exemple suivant montre comment extraire le texte d'un document sous forme de texte HTML :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraction d'un texte formaté dans le lecteur
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // Affiche un texte formaté à partir du document
        // Si l'extraction de texte formaté n'est pas supportée, un lecteur est nul
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### Voir également

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

Extrait un texte formaté de la page du document.

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | FormattedTextOptions | Les options d'extraction de texte formaté. |

### Return_Value

Une instance deTextReaderclasse avec le texte extrait ; `nul` si l'extraction de page de texte formatée n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire le texte formaté de la page du document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extraire un texte de document comme[HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extraire un texte de document comme[Réduction](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extraire un texte de document comme[Texte brut](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Exemples

L'exemple suivant montre comment extraire le texte d'une page de document sous forme de texte Markdown :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de texte formaté
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
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
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // Extraction d'un texte formaté dans le lecteur
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // Affiche un texte formaté à partir du document
            // Nous ignorons la vérification nulle car nous avons vérifié précédemment la prise en charge de la fonctionnalité d'extraction de texte formaté
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir également

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
