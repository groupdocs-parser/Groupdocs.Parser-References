---
title: "PreviewOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe PreviewOptionsgroupdocs.parser.options/previewoptions provoquant la fermeture du flux de sortie."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/previewoptions/previewoptions/
---

## PreviewOptions(CreatePageStream) {#constructor}

Initialise une nouvelle instance de la classe [`PreviewOptions`](../../previewoptions) provoquant la fermeture du flux de sortie.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| createPageStream | CreatePageStream | Crée un flux pour un aperçu de page spécifique. |

### Voir aussi

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Initialise une nouvelle instance de la classe [`PreviewOptions`](../../previewoptions) provoquant le retour du flux de sortie au client pour une utilisation ultérieure.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| createPageStream | CreatePageStream | Crée un flux pour un aperçu de page spécifique |
| releasePageStream | ReleasePageStream | Notifie que la génération de l'aperçu de page est terminée et récupère le flux de sortie. |

### Voir aussi

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
