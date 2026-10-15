---
title: "GetAnnotations"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait les annotations du document. Notez que seul le format PDF est actuellement pris en charge."
type: docs
weight: 60
url: /fr/net/groupdocs.parser/parser/getannotations/
---

## GetAnnotations() {#getannotations}

Extrait les annotations du document. Notez que seul le format PDF est actuellement pris en charge.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations()
```

### Valeur de retour

Une collection d'éléments d'annotation ; `null` si l'extraction d'annotations n'est pas prise en charge.

### Voir aussi

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetAnnotations(int) {#getannotations_1}

Extrait les annotations de la page du document. Notez que seul le format PDF est actuellement pris en charge.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une collection d'éléments d'annotation ; `null` si l'extraction d'annotations n'est pas prise en charge.

### Voir aussi

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
