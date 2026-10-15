---
title: "ParserSettings"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les paramètres qui sont utilisés pour personnaliser l'extraction de données."
type: docs
weight: 540
url: /fr/net/groupdocs.parser.options/parsersettings/
---

## ParserSettings class

Fournit les paramètres qui sont utilisés pour personnaliser l'extraction de données.

```csharp
public sealed class ParserSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ParserSettings](parsersettings#constructor)(ExternalResourceHandler) | Initialise une nouvelle instance de la classe [`ParserSettings`](../parsersettings) avec le gestionnaire de ressources externes. |
| [ParserSettings](parsersettings#constructor_1)(ILogger) | Initialise une nouvelle instance de la classe [`ParserSettings`](../parsersettings) avec le logger. |
| [ParserSettings](parsersettings#constructor_4)(OcrConnectorBase) | Initialise une nouvelle instance de la classe [`ParserSettings`](../parsersettings) avec le OCR Connector. |
| [ParserSettings](parsersettings#constructor_2)(ILogger, OcrConnectorBase) | Initialise une nouvelle instance de la classe [`ParserSettings`](../parsersettings) avec le logger et le OCR Connector. |
| [ParserSettings](parsersettings#constructor_3)(ILogger, OcrConnectorBase, ExternalResourceHandler) | Initialise une nouvelle instance de la classe [`ParserSettings`](../parsersettings) avec le logger, le OCR Connector et le gestionnaire de ressources externes. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ExternalResourceHandler](../../groupdocs.parser.options/parsersettings/externalresourcehandler) { get; } | Obtient le gestionnaire pour les ressources externes. |
| [Logger](../../groupdocs.parser.options/parsersettings/logger) { get; } | Obtient le logger utilisé pour consigner les événements et les erreurs lors de l’extraction des données. |
| [OcrConnector](../../groupdocs.parser.options/parsersettings/ocrconnector) { get; } | Obtient le OCR Connector utilisé pour fournir la fonctionnalité OCR. |

### Remarques

**Learn more:**

* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
