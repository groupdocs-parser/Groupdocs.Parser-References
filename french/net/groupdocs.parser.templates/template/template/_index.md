---
title: "Modèle"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe Templategroupdocs.parser.templates/template."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.templates/template/template/
---

## Template(IEnumerable&lt;TemplateItem&gt;) {#constructor}

Initialise une nouvelle instance de la classe [`Template`](../../template).

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| items | IEnumerable`1 | La collection d'objets [`TemplateItem`](../../templateitem). |

### Exemples

Utilisation :

```csharp
// Créez un tableau de champs de modèle
TemplateItem[] fields = new TemplateItem[]
{
   new TemplateField(new TemplateRegexPosition("From"), "From", 0),
   new TemplateField(
       new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromCompany",
       0),
   new TemplateField(
       new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromAddress",
       0)
};

// Créer un modèle de document
Template template = new Template(fields);
```

### Voir aussi

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Template(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`Template`](../../template) avec des options de modèle.

```csharp
public Template(IEnumerable<TemplateItem> items, TemplateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| items | IEnumerable`1 | La collection d'objets [`TemplateItem`](../../templateitem). |
| options | TemplateOptions | Les options du modèle. |

### Voir aussi

* class [TemplateItem](../../templateitem)
* class [TemplateOptions](../../templateoptions)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
