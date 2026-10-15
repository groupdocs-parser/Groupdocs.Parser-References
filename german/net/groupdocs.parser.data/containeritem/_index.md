---
title: "ContainerItem"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt ein Container-Element dar, wie z. B. ein ZIP-Archiv, eine E‑Mail‑Anlage, ein PDF‑Portfolio‑Element und so weiter."
type: docs
weight: 720
url: /de/net/groupdocs.parser.data/containeritem/
---

## ContainerItem class

Stellt ein Containerelement dar, wie z. B. ein Zip‑Archiv‑Entität, E‑Mail‑Anhang, PDF‑Portfolio‑Element und so weiter.

```csharp
public sealed class ContainerItem
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | Liefert das Verzeichnis des Elements. |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | Liefert den vollständigen Pfad des Elements. |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | Liefert die Sammlung der Metadatenobjekte. |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | Liefert den Namen des Elements. |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | Ermittelt die Größe des Elements. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | Erkennt den Dateityp des Container-Elements. |
| [GetMetadataValue](../../groupdocs.parser.data/containeritem/getmetadatavalue)(string) | Ermittelt den Metadatenwert. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | Erstellt das [`Parser`](../../groupdocs.parser/parser)-Objekt für den Inhalt des Elements. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | Erstellt das [`Parser`](../../groupdocs.parser/parser)-Objekt für den Inhalt des Elements mit [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | Erstellt das [`Parser`](../../groupdocs.parser/parser)-Objekt für den Inhalt des Elements mit [`LoadOptions`](../../groupdocs.parser.options/loadoptions) und [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | Öffnet den Stream des Elementinhalts. |

### Hinweise

Eine Instanz der Klasse [`ContainerItem`](../containeritem) wird als Rückgabewert der Methode [`GetContainer`](../../groupdocs.parser/parser/getcontainer) verwendet. Siehe dort die Anwendungsbeispiele.

### Siehe auch

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
