---
title: Metadata
second_title: GroupDocs.Parser voor .NET API-referentie
description: Haalt de verzameling metadataitems op.
type: docs
weight: 30
url: /nl/net/groupdocs.parser.data/containeritem/metadata/
---
## ContainerItem.Metadata property

Haalt de verzameling metadata-items op.

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Eigendoms-waarde

Een verzameling van[`MetadataItem`](../../metadataitem) voorwerpen; leeg als metadata niet is ingesteld.

### Opmerkingen

Deze metadata verwijzen naar een containerelement zelf, niet naar een document. Afhankelijk van het containertype kunnen metadata de volgende items bevatten:

**E-mailbijlagen**

**Naam**

**Beschrijving**

**inhoudstype**

Het MIME-type van de bijlage-inhoud.

**ZIP-archieven**

**Naam**

**Beschrijving**

**datum**

De tijd en datum waarop het bestand aangegeven door de Zip-invoer voor het laatst is gewijzigd.

**Outlook-opslag**

**Naam**

**Beschrijving**

**datum**

De tijd en datum waarop het Outlook-opslagitem voor het laatst is gewijzigd.

**e-mail afzender**

De waarde van het veld "afzender".

**email naar**

De waarde van het veld "naar".

**onderwerp**

De waarde van het veld "onderwerp".

### Zie ook

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* naamruimte [GroupDocs.Parser.Data](../../containeritem)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
