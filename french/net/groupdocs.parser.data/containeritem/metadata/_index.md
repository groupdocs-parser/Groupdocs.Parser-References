---
title: "Métadonnées"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Obtient la collection d'éléments de métadonnées."
type: docs
weight: 30
url: /fr/net/groupdocs.parser.data/containeritem/metadata/
---

## ContainerItem.Metadata property

Obtient la collection d'éléments de métadonnées.

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Property Value

Une collection d'objets [`MetadataItem`](../../metadataitem) ; vide si les métadonnées ne sont pas définies.

### Remarques

Ces métadonnées se réfèrent à l'élément conteneur lui‑même, pas à un document. Selon le type de conteneur, les métadonnées peuvent contenir les éléments suivants :

**Email Attachments**

**Name**

**Description**

**content-type**

Le type MIME du contenu de la pièce jointe.

**ZIP Archives**

**Name**

**Description**

**date**

La date et l'heure auxquelles le fichier indiqué par l'entrée Zip a été modifié pour la dernière fois.

**disposition**

Pour détecter si la pièce jointe image est en ligne, les métadonnées de « disposition » sont utilisées. Si elles sont présentes, elles peuvent prendre les valeurs « inline » ou « attachment ».

**Outlook Storage**

**Name**

**Description**

**date**

La date et l'heure auxquelles l'élément Outlook Storage a été modifié pour la dernière fois.

**email-sender**

La valeur du champ « sender ».

**email-to**

La valeur du champ « to ».

**subject**

La valeur du champ « subject ».

### Voir aussi

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
