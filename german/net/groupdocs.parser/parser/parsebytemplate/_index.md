---
title: "ParseByTemplate"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Parst das Dokument anhand der benutzergenerierten Vorlage."
type: docs
weight: 230
url: /de/net/groupdocs.parser/parser/parsebytemplate/
---

## ParseByTemplate(Template) {#parsebytemplate}

Parst das Dokument anhand der vom Benutzer erstellten Vorlage.

```csharp
public DocumentData ParseByTemplate(Template template)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| template | Template | Die benutzergenerierte Vorlage. |

### Rückgabewert

Eine Instanz der [`DocumentData`](../../../groupdocs.parser.data/documentdata)-Klasse, die die extrahierten Daten enthält; `null`, wenn das Parsen anhand einer Vorlage nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(Template, ParseByTemplateOptions) {#parsebytemplate_1}

Parst das Dokument anhand der vom Benutzer erstellten Vorlage unter Verwendung von Anpassungsoptionen.

```csharp
public DocumentData ParseByTemplate(Template template, ParseByTemplateOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| template | Template | Die benutzergenerierte Vorlage. |
| options | ParseByTemplateOptions | Die Anpassungsoptionen. |

### Rückgabewert

Eine Instanz der [`DocumentData`](../../../groupdocs.parser.data/documentdata)-Klasse, die die extrahierten Daten enthält; `null`, wenn das Parsen anhand einer Vorlage nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(TemplateCollection, ParseByTemplateOptions) {#parsebytemplate_2}

Wählt die am besten geeignete Vorlage aus der bereitgestellten Sammlung aus und parst anschließend das Dokument anhand der ausgewählten Vorlage.

```csharp
public DocumentData ParseByTemplate(TemplateCollection templateCollection, 
    ParseByTemplateOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateCollection | TemplateCollection | Die Vorlagensammlung. |
| options | ParseByTemplateOptions | Die Anpassungsoptionen. |

### Rückgabewert

Eine Instanz der [`DocumentData`](../../../groupdocs.parser.data/documentdata)-Klasse, die die extrahierten Daten enthält; `null`, wenn das Parsen anhand einer Vorlage nicht unterstützt wird.

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [TemplateCollection](../../../groupdocs.parser.templates/templatecollection)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
