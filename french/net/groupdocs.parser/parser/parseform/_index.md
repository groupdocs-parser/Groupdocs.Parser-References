---
title: "ParseForm"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Analyse le formulaire du document."
type: docs
weight: 240
url: /fr/net/groupdocs.parser/parser/parseform/
---

## Parser.ParseForm method

Analyse le formulaire du document.

```csharp
public DocumentData ParseForm()
```

### Valeur de retour

Une instance de la classe [`DocumentData`](../../../groupdocs.parser.data/documentdata) qui contient les données extraites ; `null` si l'analyse par modèle n'est pas prise en charge.

### Remarques

**Learn more:**

* [Extract data from PDF forms](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [Working with extracted data](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Exemples

L'exemple suivant montre comment analyser un formulaire du document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire les données du document PDF
    DocumentData data = parser.ParseForm();
    // Parcourir les données extraites
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
