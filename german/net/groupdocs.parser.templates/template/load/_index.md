---
title: "Load"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Lädt eine Vorlage aus einer Datei."
type: docs
weight: 20
url: /de/net/groupdocs.parser.templates/template/load/
---

## Load(string) {#load_1}

Lädt eine Vorlage aus einer Datei.

```csharp
public static Template Load(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |

### Rückgabewert

Eine Instanz der [`Template`](../../template) Klasse mit geladener Vorlage.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Die Datei stellt die Vorlage nicht in einem gültigen Format dar. |

### Siehe auch

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Load(Stream) {#load}

Lädt eine Vorlage aus einem Stream.

```csharp
public static Template Load(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Eingabestream. |

### Rückgabewert

Eine Instanz der [`Template`](../../template) Klasse mit geladener Vorlage.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Der Stream stellt die Vorlage nicht in einem gültigen Format dar. |

### Siehe auch

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
