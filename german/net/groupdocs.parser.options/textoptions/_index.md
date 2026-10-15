---
title: "TextOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für die Textextraktion verwendet werden."
type: docs
weight: 610
url: /de/net/groupdocs.parser.options/textoptions/
---

## TextOptions class

Stellt die Optionen bereit, die für die Textextraktion verwendet werden.

```csharp
public sealed class TextOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TextOptions](textoptions#constructor)() | Initialisiert eine neue Instanz der [`TextOptions`](../textoptions)-Klasse. |
| [TextOptions](textoptions#constructor_1)(bool) | Initialisiert eine neue Instanz der [`TextOptions`](../textoptions)-Klasse. |
| [TextOptions](textoptions#constructor_2)(bool, bool) | Initialisiert eine neue Instanz der [`TextOptions`](../textoptions)-Klasse mit der OCR-Nutzungsoption. |
| [TextOptions](textoptions#constructor_3)(bool, bool, OcrOptions) | Initialisiert eine neue Instanz der [`TextOptions`](../textoptions)-Klasse mit der Möglichkeit, OCR-Optionen festzulegen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IncludeAnnotations](../../groupdocs.parser.options/textoptions/includeannotations) { get; set; } | Gibt den Wert zurück, der angibt, ob Anmerkungen enthalten sind. Der Standardwert ist `false`. |
| [OcrOptions](../../groupdocs.parser.options/textoptions/ocroptions) { get; set; } | Gibt die zusätzlichen Optionen für die OCR-Funktionalität zurück. |
| [UseOcr](../../groupdocs.parser.options/textoptions/useocr) { get; set; } | Gibt den Wert zurück, der angibt, ob der OCR Connector verwendet wird, um einen Text zu extrahieren. |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; set; } | Gibt den Wert zurück, der angibt, ob der Rohmodus verwendet wird. |

### Hinweise

Eine Instanz der [`TextOptions`](../textoptions)-Klasse wird als Parameter in den Methoden [`GetText`](../../groupdocs.parser/parser/gettext) und [`GetText`](../../groupdocs.parser/parser/gettext) verwendet. Siehe dort die Anwendungsbeispiele.

Sie wird verwendet, um den Rohmodus der Textextraktion anzugeben. Ein Text in diesem Modus wird auf ungenaue Weise, aber schneller als im Standardmodus extrahiert. Wenn der Rohmodus das Dokumentformat nicht unterstützt, wird dieser Parameter ignoriert und der Standardmodus verwendet.

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
