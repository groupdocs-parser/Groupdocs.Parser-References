---
title: "GetPagePreview"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Erstellt eine Vorschau der Dokumentseite."
type: docs
weight: 150
url: /de/net/groupdocs.parser/parser/getpagepreview/
---

## GetPagePreview(int) {#getpagepreview}

Erstellt eine Vorschau der Dokumentseite.

```csharp
public Stream GetPagePreview(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Instanz von Stream, die ein Bild der Dokumentenseite enthält; `null`, wenn die Generierung der Seitenvorschau nicht unterstützt wird.

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetPagePreview(int, PagePreviewOptions) {#getpagepreview_1}

Erstellt eine Vorschau der Dokumentseite mithilfe von Anpassungsoptionen.

```csharp
public Stream GetPagePreview(int pageIndex, PagePreviewOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PagePreviewOptions | Die Optionen, um die Vorschaugenerierung anzupassen. |

### Rückgabewert

Eine Instanz von Stream, die ein Bild der Dokumentenseite enthält; `null`, wenn die Generierung der Seitenvorschau nicht unterstützt wird.

### Siehe auch

* class [PagePreviewOptions](../../../groupdocs.parser.options/pagepreviewoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
