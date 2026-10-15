---
title: "ReleasePageStream"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt eine Methode dar, die den von dem CreatePageStream./createpagestream-Delegaten erstellten Stream freigibt."
type: docs
weight: 580
url: /de/net/groupdocs.parser.options/releasepagestream/
---

## ReleasePageStream delegate

Stellt eine Methode dar, die den von dem [`CreatePageStream`](../createpagestream)-Delegaten erstellten Stream freigibt.

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageNumber | Int32 | Die Seitennummer einer erzeugten Seitenvorschau. |
| pageStream | Stream | Der Stream, der die erzeugte Seitenvorschau enthält. |

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
