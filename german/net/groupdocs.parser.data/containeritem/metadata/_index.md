---
title: "Metadaten"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Liefert die Sammlung der Metadatenobjekte."
type: docs
weight: 30
url: /de/net/groupdocs.parser.data/containeritem/metadata/
---

## ContainerItem.Metadata property

Liefert die Sammlung der Metadatenobjekte.

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Property Value

Eine Sammlung von [`MetadataItem`](../../metadataitem)-Objekten; leer, wenn Metadaten nicht gesetzt sind.

### Hinweise

Diese Metadaten beziehen sich auf das Containerelement selbst, nicht auf ein Dokument. Abhängig vom Containertyp können Metadaten die folgenden Elemente enthalten:

**Email Attachments**

**Name**

**Description**

**content-type**

Der MIME-Typ des Anhangsinhalts.

**ZIP Archives**

**Name**

**Description**

**date**

Zeit und Datum, zu denen die durch den Zip-Eintrag angegebene Datei zuletzt geändert wurde.

**disposition**

Um zu erkennen, ob ein Bildanhang inline ist, wird die Metadaten-'Disposition' verwendet. Wenn sie vorhanden ist, kann sie die Werte 'inline' oder 'attachment' annehmen.

**Outlook Storage**

**Name**

**Description**

**date**

Zeit und Datum, zu denen das Outlook‑Speicherelement zuletzt geändert wurde.

**email-sender**

Der Wert des Feldes "sender".

**email-to**

Der Wert des Feldes "to".

**subject**

Der Wert des Feldes "subject".

### Siehe auch

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
