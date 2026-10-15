---
title: "PreviewOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der PreviewOptionsgroupdocs.parser.options/previewoptions-Klasse, wodurch der Ausgabestream geschlossen wird."
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/previewoptions/previewoptions/
---

## PreviewOptions(CreatePageStream) {#constructor}

Initialisiert eine neue Instanz der [`PreviewOptions`](../../previewoptions)-Klasse, wodurch der Ausgabestream geschlossen wird.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| createPageStream | CreatePageStream | Erstellt einen Stream für eine bestimmte Seitenvorschau. |

### Siehe auch

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Initialisiert eine neue Instanz der [`PreviewOptions`](../../previewoptions)-Klasse, wodurch der Ausgabestream dem Client für weitere Verwendung zurückgegeben wird.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| createPageStream | CreatePageStream | Erstellt einen Stream für eine bestimmte Seitenvorschau |
| releasePageStream | ReleasePageStream | Benachrichtigt, dass die Erzeugung der Seitenvorschau abgeschlossen ist, und gibt den Ausgabestream zurück. |

### Siehe auch

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
