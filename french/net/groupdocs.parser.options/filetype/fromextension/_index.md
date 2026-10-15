---
title: "FromExtension"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Mappe l'extension de fichier au type de fichier."
type: docs
weight: 930
url: /fr/net/groupdocs.parser.options/filetype/fromextension/
---

## FileType.FromExtension method

Mappe l'extension de fichier au type de fichier.

```csharp
public static FileType FromExtension(string extension)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| extension | Chaîne | Extension de fichier (y compris le point "."). |

### Valeur de retour

Lorsque le type de fichier est pris en charge, le renvoie, sinon renvoie le type de fichier par défaut [`Unknown`](../unknown).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lancée lorsque *extension* est null ou une chaîne vide. |

### Voir aussi

* class [FileType](../../filetype)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
