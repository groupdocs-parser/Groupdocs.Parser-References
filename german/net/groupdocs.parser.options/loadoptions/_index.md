---
title: "LoadOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die zum Öffnen einer Datei verwendet werden."
type: docs
weight: 420
url: /de/net/groupdocs.parser.options/loadoptions/
---

## LoadOptions class

Stellt die Optionen bereit, die zum Öffnen einer Datei verwendet werden.

```csharp
public sealed class LoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit leerem [`Password`](./password), [`FileFormat`](./fileformat) gleich Unknown und Standardkodierungen. |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit leerem [`Password`](./password) und Standardkodierungen. |
| [LoadOptions](loadoptions#constructor_5)(FileType) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit leerem [`Password`](./password) und Standardkodierungen. |
| [LoadOptions](loadoptions#constructor_9)(string) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit [`FileFormat`](./fileformat) gleich Unknown und Standardkodierungen. |
| [LoadOptions](loadoptions#constructor_10)(TimeSpan) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit *timeout*. |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit dem Passwort und Standardkodierungen. |
| [LoadOptions](loadoptions#constructor_6)(FileType, string) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit dem Passwort und Standardkodierungen. |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit benutzerdefinierten Kodierungen. |
| [LoadOptions](loadoptions#constructor_7)(FileType, string, Encoding, Encoding) | Initialisiert eine neue Instanz der [`LoadOptions`](../loadoptions)-Klasse mit benutzerdefinierten Kodierungen. |
| [LoadOptions](loadoptions#constructor_4)(FileFormat, string, Encoding, Encoding, TimeSpan) | Initialisiert eine neue Instanz der vollständig angepassten [`LoadOptions`](../loadoptions)-Klasse. |
| [LoadOptions](loadoptions#constructor_8)(FileType, string, Encoding, Encoding, TimeSpan) | Initialisiert eine neue Instanz der vollständig angepassten [`LoadOptions`](../loadoptions)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | Ruft die standardmäßige ANSI-Kodierung ab, die für die Kodierungserkennung verwendet wird. |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | Ruft die Kodierung des Dokuments ab. |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | Ruft das Dateiformat ab. |
| [FileType](../../groupdocs.parser.options/loadoptions/filetype) { get; } | Ruft den Dateityp ab. |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | Ermittelt das Passwort. |
| [Timeout](../../groupdocs.parser.options/loadoptions/timeout) { get; } | Ruft den Wert ab, der die Anzahl der Millisekunden zum Warten darstellt. |

### Hinweise

Eine Instanz dieser Klasse wird als Parameter in den Konstruktoren der [`Parser`](../../groupdocs.parser/parser)-Klasse verwendet:

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
