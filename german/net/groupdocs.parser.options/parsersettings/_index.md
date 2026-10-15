---
title: "ParserSettings"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Einstellungen bereit, die zur Anpassung der Datenextraktion verwendet werden."
type: docs
weight: 540
url: /de/net/groupdocs.parser.options/parsersettings/
---

## ParserSettings class

Stellt die Einstellungen bereit, die zur Anpassung der Datenextraktion verwendet werden.

```csharp
public sealed class ParserSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ParserSettings](parsersettings#constructor)(ExternalResourceHandler) | Initialisiert eine neue Instanz der [`ParserSettings`](../parsersettings)-Klasse mit dem External Resource Handler. |
| [ParserSettings](parsersettings#constructor_1)(ILogger) | Initialisiert eine neue Instanz der [`ParserSettings`](../parsersettings)-Klasse mit dem Logger. |
| [ParserSettings](parsersettings#constructor_4)(OcrConnectorBase) | Initialisiert eine neue Instanz der [`ParserSettings`](../parsersettings)-Klasse mit dem OCR Connector. |
| [ParserSettings](parsersettings#constructor_2)(ILogger, OcrConnectorBase) | Initialisiert eine neue Instanz der [`ParserSettings`](../parsersettings)-Klasse mit Logger und OCR Connector. |
| [ParserSettings](parsersettings#constructor_3)(ILogger, OcrConnectorBase, ExternalResourceHandler) | Initialisiert eine neue Instanz der [`ParserSettings`](../parsersettings)-Klasse mit Logger, OCR Connector und External Resource Handler. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ExternalResourceHandler](../../groupdocs.parser.options/parsersettings/externalresourcehandler) { get; } | Gibt den Handler für externe Ressourcen zurück. |
| [Logger](../../groupdocs.parser.options/parsersettings/logger) { get; } | Gibt den Logger zurück, der für das Protokollieren von Ereignissen und Fehlern während der Datenextraktion verwendet wird. |
| [OcrConnector](../../groupdocs.parser.options/parsersettings/ocrconnector) { get; } | Gibt den OCR Connector zurück, der verwendet wird, um OCR-Funktionalität bereitzustellen. |

### Hinweise

**Learn more:**

* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
