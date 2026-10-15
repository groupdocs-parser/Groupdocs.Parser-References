---
title: "ParseByTemplate"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Analyse le document à l'aide du modèle généré par l'utilisateur."
type: docs
weight: 230
url: /fr/net/groupdocs.parser/parser/parsebytemplate/
---

## ParseByTemplate(Template) {#parsebytemplate}

Analyse le document à l'aide du modèle généré par l'utilisateur.

```csharp
public DocumentData ParseByTemplate(Template template)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| template | Modèle | Le modèle généré par l'utilisateur. |

### Valeur de retour

Une instance de la classe [`DocumentData`](../../../groupdocs.parser.data/documentdata) qui contient les données extraites ; `null` si l'analyse par modèle n'est pas prise en charge.

### Remarques

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(Template, ParseByTemplateOptions) {#parsebytemplate_1}

Analyse le document à l'aide du modèle généré par l'utilisateur en utilisant des options de personnalisation.

```csharp
public DocumentData ParseByTemplate(Template template, ParseByTemplateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| template | Modèle | Le modèle généré par l'utilisateur. |
| options | ParseByTemplateOptions | Les options de personnalisation. |

### Valeur de retour

Une instance de la classe [`DocumentData`](../../../groupdocs.parser.data/documentdata) qui contient les données extraites ; `null` si l'analyse par modèle n'est pas prise en charge.

### Remarques

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(TemplateCollection, ParseByTemplateOptions) {#parsebytemplate_2}

Sélectionne le modèle le plus adapté parmi la collection fournie, puis analyse le document selon le modèle sélectionné.

```csharp
public DocumentData ParseByTemplate(TemplateCollection templateCollection, 
    ParseByTemplateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateCollection | TemplateCollection | La collection de modèles. |
| options | ParseByTemplateOptions | Les options de personnalisation. |

### Valeur de retour

Une instance de la classe [`DocumentData`](../../../groupdocs.parser.data/documentdata) qui contient les données extraites ; `null` si l'analyse par modèle n'est pas prise en charge.

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [TemplateCollection](../../../groupdocs.parser.templates/templatecollection)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
