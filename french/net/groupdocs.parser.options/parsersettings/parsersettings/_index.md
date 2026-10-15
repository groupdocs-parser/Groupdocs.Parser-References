---
title: "ParserSettings"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe ParserSettingsgroupdocs.parser.options/parsersettings avec le logger."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/parsersettings/parsersettings/
---

## ParserSettings(ILogger) {#constructor_1}

Initialise une nouvelle instance de la classe [`ParserSettings`](../../parsersettings) avec le logger.

```csharp
public ParserSettings(ILogger logger)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| logger | ILogger | Une instance de classe qui implémente l'interface [`ILogger`](../../ilogger). |

### Voir aussi

* interface [ILogger](../../ilogger)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(OcrConnectorBase) {#constructor_4}

Initialise une nouvelle instance de la classe [`ParserSettings`](../../parsersettings) avec le connecteur OCR.

```csharp
public ParserSettings(OcrConnectorBase ocrConnector)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ocrConnector | OcrConnectorBase | Une instance de classe qui hérite de la classe [`OcrConnectorBase`](../../ocrconnectorbase) pour fournir la fonctionnalité OCR. |

### Voir aussi

* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ExternalResourceHandler) {#constructor}

Initialise une nouvelle instance de la classe [`ParserSettings`](../../parsersettings) avec le gestionnaire de ressources externes.

```csharp
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| externalResourceHandler | ExternalResourceHandler | Une instance de classe qui hérite de la classe [`ExternalResourceHandler`](../../externalresourcehandler) pour fournir le contrôle du chargement des ressources externes. |

### Voir aussi

* class [ExternalResourceHandler](../../externalresourcehandler)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase) {#constructor_2}

Initialise une nouvelle instance de la classe [`ParserSettings`](../../parsersettings) avec le journaliseur et le connecteur OCR.

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| logger | ILogger | Une instance de classe qui implémente l'interface [`ILogger`](../../ilogger). |
| ocrConnector | OcrConnectorBase | Une instance de classe qui hérite de la classe [`OcrConnectorBase`](../../ocrconnectorbase) pour fournir la fonctionnalité OCR. |

### Voir aussi

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase, ExternalResourceHandler) {#constructor_3}

Initialise une nouvelle instance de la classe [`ParserSettings`](../../parsersettings) avec le journaliseur, le connecteur OCR et le gestionnaire de ressources externes.

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, 
    ExternalResourceHandler externalResourceHandler)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| logger | ILogger | Une instance de classe qui implémente l'interface [`ILogger`](../../ilogger). |
| ocrConnector | OcrConnectorBase | Une instance de classe qui hérite de la classe [`OcrConnectorBase`](../../ocrconnectorbase) pour fournir la fonctionnalité OCR. |
| externalResourceHandler | ExternalResourceHandler | Une instance de classe qui hérite de la classe [`ExternalResourceHandler`](../../externalresourcehandler) pour fournir le contrôle du chargement des ressources externes. |

### Voir aussi

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ExternalResourceHandler](../../externalresourcehandler)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
