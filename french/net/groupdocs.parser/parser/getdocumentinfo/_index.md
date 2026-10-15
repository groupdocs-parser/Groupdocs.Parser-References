---
title: "GetDocumentInfo"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Renvoie les informations générales sur le document."
type: docs
weight: 90
url: /fr/net/groupdocs.parser/parser/getdocumentinfo/
---

## Parser.GetDocumentInfo method

Renvoie les informations générales sur le document.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Valeur de retour

Une instance d'une classe qui implémente l'interface [`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo).

### Remarques

**Learn more:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Exemples

L'exemple suivant montre comment obtenir les informations du document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Obtenir les informations du document
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### Voir aussi

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
