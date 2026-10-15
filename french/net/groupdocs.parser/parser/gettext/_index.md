---
title: "GetText"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait un texte du document."
type: docs
weight: 180
url: /fr/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Extrait un texte du document.

```csharp
public TextReader GetText()
```

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait ; `null` si l'extraction de texte n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Exemples

L'exemple suivant montre comment extraire du texte d'un document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire du texte dans le lecteur
    using(TextReader reader = parser.GetText())
    {
        // Afficher du texte depuis le document
        // Si l'extraction de texte n'est pas prise en charge, le lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extrait une page de texte du document en utilisant les options de texte (pour activer le mode d'extraction de texte brut rapide).

```csharp
public TextReader GetText(TextOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | TextOptions | Les options d'extraction de texte. |

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait ; `null` si l'extraction de texte n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Exemples

L'exemple suivant montre comment extraire du texte brut d'un document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Extraire du texte brut dans le lecteur
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Afficher du texte depuis le document
        // Si l'extraction de texte n'est pas prise en charge, le lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir aussi

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extrait un texte de la page du document.

```csharp
public TextReader GetText(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait ; `null` si l'extraction de texte de page n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Exemples

L'exemple suivant montre comment extraire du texte de la page du document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de texte
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extraire du texte dans le lecteur
        using(TextReader reader = parser.GetText(p))
        {
            // Afficher du texte depuis le document
            // Nous ignorons la vérification de null car nous avons déjà vérifié la prise en charge de la fonction d'extraction de texte.
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extrait un texte de la page du document en utilisant les options de texte (pour activer le mode d'extraction de texte brut rapide).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | TextOptions | Les options d'extraction de texte. |

### Valeur de retour

Une instance de la classe TextReader contenant le texte extrait ; `null` si l'extraction de texte de page n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Exemples

L'exemple suivant montre comment extraire du texte brut de la page du document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de texte
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Obtenir les informations du document
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Vérifier si le document possède des pages
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Parcourir les pages
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extraire du texte dans le lecteur
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Afficher du texte depuis le document
            // Nous ignorons la vérification de null car nous avons déjà vérifié la prise en charge de la fonction d'extraction de texte.
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
