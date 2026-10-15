---
title: "GetAnnotations"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert Anmerkungen aus dem Dokument. Hinweis: Derzeit wird nur das PDF‑Format unterstützt."
type: docs
weight: 60
url: /de/net/groupdocs.parser/parser/getannotations/
---

## GetAnnotations() {#getannotations}

Extrahiert Anmerkungen aus dem Dokument. Hinweis: Derzeit wird nur das PDF‑Format unterstützt.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations()
```

### Rückgabewert

Eine Sammlung von Annotations‑Elementen; `null`, wenn die Annotationsextraktion nicht unterstützt wird.

### Siehe auch

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetAnnotations(int) {#getannotations_1}

Extrahiert Anmerkungen von der Dokumentenseite. Hinweis: Derzeit wird nur das PDF‑Format unterstützt.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von Annotations‑Elementen; `null`, wenn die Annotationsextraktion nicht unterstützt wird.

### Siehe auch

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
