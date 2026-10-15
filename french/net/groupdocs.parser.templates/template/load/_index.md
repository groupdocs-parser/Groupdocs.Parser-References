---
title: "Load"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Charge un modèle depuis un fichier."
type: docs
weight: 20
url: /fr/net/groupdocs.parser.templates/template/load/
---

## Load(string) {#load_1}

Charge un modèle depuis un fichier.

```csharp
public static Template Load(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |

### Valeur de retour

Une instance de la classe [`Template`](../../template) avec le modèle chargé.

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Le fichier ne représente pas le modèle dans un format valide. |

### Voir aussi

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Load(Stream) {#load}

Charge un modèle depuis un flux.

```csharp
public static Template Load(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Stream | Le flux d'entrée. |

### Valeur de retour

Une instance de la classe [`Template`](../../template) avec le modèle chargé.

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Le flux ne représente pas le modèle dans un format valide. |

### Voir aussi

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
