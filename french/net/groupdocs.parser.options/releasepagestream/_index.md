---
title: "ReleasePageStream"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente une méthode qui libère le flux créé par le délégué CreatePageStream./createpagestream."
type: docs
weight: 580
url: /fr/net/groupdocs.parser.options/releasepagestream/
---

## ReleasePageStream delegate

Représente une méthode qui libère le flux créé par le délégué [`CreatePageStream`](../createpagestream).

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageNumber | Int32 | Le numéro de page d'un aperçu de page généré. |
| pageStream | Stream | Le flux contenant l'aperçu de page généré. |

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
