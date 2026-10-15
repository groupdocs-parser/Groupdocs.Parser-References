---
title: "GetFieldsByName"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Renvoie la collection des données de champ dont le nom est égal à fieldName."
type: docs
weight: 50
url: /fr/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---

## DocumentData.GetFieldsByName method

Renvoie la collection de données de champ dont le nom est égal à *fieldName*.

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | Chaîne | Le nom du champ. |

### Valeur de retour

Une collection d'objets [`FieldData`](../../fielddata) ; collection vide si aucune donnée de champ n'est trouvée.

### Exemples

Trouver les champs par un nom de champ :

```csharp
// Obtenir tous les champs portant le nom "Address"
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // Itérer sur la collection de champs
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // Si c'est un champ lié :
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields.

### Voir aussi

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
