---
title: "Template"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Templategroupdocs.parser.templates/template Klasse."
type: docs
weight: 10
url: /de/net/groupdocs.parser.templates/template/template/
---

## Template(IEnumerable&lt;TemplateItem&gt;) {#constructor}

Initialisiert eine neue Instanz der [`Template`](../../template) Klasse.

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| items | IEnumerable`1 | Die Sammlung von [`TemplateItem`](../../templateitem) Objekten. |

### Beispiele

Verwendung:

```csharp
// Erstellen Sie ein Array von Vorlagenfeldern
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

// Erstelle eine Dokumentvorlage
Template template = new Template(fields);
```

### Siehe auch

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Template(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`Template`](../../template)-Klasse mit Vorlagenoptionen.

```csharp
public Template(IEnumerable<TemplateItem> items, TemplateOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| items | IEnumerable`1 | Die Sammlung von [`TemplateItem`](../../templateitem) Objekten. |
| options | TemplateOptions | Die Vorlagenoptionen. |

### Siehe auch

* class [TemplateItem](../../templateitem)
* class [TemplateOptions](../../templateoptions)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
