---
title: "Fonctionnalités"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Obtient les fonctionnalités prises en charge."
type: docs
weight: 20
url: /fr/net/groupdocs.parser/parser/features/
---

## Parser.Features property

Obtient les fonctionnalités prises en charge.

```csharp
public Features Features { get; }
```

### Property Value

Une instance de la classe [`Features`](../../../groupdocs.parser.options/features) qui représente les fonctionnalités prises en charge.

### Remarques

**Learn more:**

* [Get supported features](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### Exemples

Si la fonctionnalité n'est pas prise en charge, la méthode renvoie `null` au lieu de la valeur. Certaines opérations peuvent prendre un temps considérable. Il n'est donc pas optimal d'appeler la méthode uniquement pour vérifier la prise en charge de la fonctionnalité. À cette fin, la propriété Features est utilisée :

```csharp
using(Parser parser = new Parser("doc.zip"))
{
    if(!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported");
        return;
    }
 
    using(TextReader reader = parser.GetText())
    {
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

### Voir aussi

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
