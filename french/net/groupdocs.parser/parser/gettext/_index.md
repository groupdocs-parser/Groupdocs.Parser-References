---
title: GetText
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait un texte du document.
type: docs
weight: 150
url: /fr/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Extrait un texte du document.

```csharp
public TextReader GetText()
```

### Return_Value

Une instance deTextReader classe avec le texte extrait ; `nul` si l'extraction de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire du texte de documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extraire du texte en mode précis](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Exemples

L'exemple suivant montre comment extraire un texte d'un document :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire un texte dans le lecteur
    using(TextReader reader = parser.GetText())
    {
        // Imprime un texte du document
        // Si l'extraction de texte n'est pas supportée, un lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir également

* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extrait une page de texte du document à l'aide des options de texte (pour activer le mode d'extraction rapide de texte brut).

```csharp
public TextReader GetText(TextOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | TextOptions | Les options d'extraction de texte. |

### Return_Value

Une instance deTextReader classe avec le texte extrait ; `nul` si l'extraction de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire du texte en mode précis](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraire du texte en mode brut](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Exemples

L'exemple suivant montre comment extraire un texte brut d'un document :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire un texte brut dans le lecteur
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Imprime un texte du document
        // Si l'extraction de texte n'est pas supportée, un lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir également

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extrait un texte de la page du document.

```csharp
public TextReader GetText(int pageIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |

### Return_Value

Une instance deTextReader classe avec le texte extrait ; `nul` si l'extraction de page de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire du texte en mode précis](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Exemples

L'exemple suivant montre comment extraire un texte de la page du document :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de texte
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extraire un texte dans le lecteur
        using(TextReader reader = parser.GetText(p))
        {
            // Imprime un texte du document
            // Nous ignorons la vérification nulle car nous avons vérifié la prise en charge de la fonctionnalité d'extraction de texte plus tôt
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir également

* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extrait un texte de la page du document à l'aide des options de texte (pour activer le mode d'extraction rapide de texte brut).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | TextOptions | Les options d'extraction de texte. |

### Return_Value

Une instance deTextReader classe avec le texte extrait ; `nul` si l'extraction de page de texte n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Extraire du texte en mode précis](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraire du texte en mode brut](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Exemples

L'exemple suivant montre comment extraire un texte brut de la page du document :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de texte
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Récupère les informations sur le document
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Vérifie si le document contient des pages
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itérer sur les pages
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extraire un texte dans le lecteur
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Imprime un texte du document
            // Nous ignorons la vérification nulle car nous avons vérifié la prise en charge de la fonctionnalité d'extraction de texte plus tôt
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir également

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
