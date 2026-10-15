---
title: "GetPagePreview"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Génère un aperçu de la page du document."
type: docs
weight: 150
url: /fr/net/groupdocs.parser/parser/getpagepreview/
---

## GetPagePreview(int) {#getpagepreview}

Génère un aperçu de la page du document.

```csharp
public Stream GetPagePreview(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une instance de Stream contenant une image de la page du document ; `null` si la génération d'aperçu de page n'est pas prise en charge.

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetPagePreview(int, PagePreviewOptions) {#getpagepreview_1}

Génère un aperçu de la page du document en utilisant des options de personnalisation.

```csharp
public Stream GetPagePreview(int pageIndex, PagePreviewOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | PagePreviewOptions | Les options pour personnaliser la génération de l'aperçu. |

### Valeur de retour

Une instance de Stream contenant une image de la page du document ; `null` si la génération d'aperçu de page n'est pas prise en charge.

### Voir aussi

* class [PagePreviewOptions](../../../groupdocs.parser.options/pagepreviewoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
