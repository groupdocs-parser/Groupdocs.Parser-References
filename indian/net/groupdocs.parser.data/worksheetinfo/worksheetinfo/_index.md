---
title: "WorksheetInfo"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "WorksheetInfogroupdocs.parser.data/worksheetinfo क्लास का एक नया इंस्टेंस प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---

## WorksheetInfo constructor

[`WorksheetInfo`](../../worksheetinfo) क्लास का एक नया इंस्टेंस प्रारंभ करता है।

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| index | Int32 | वर्कशीट का शून्य-आधारित सूचकांक। |
| name | स्ट्रिंग | एक स्ट्रिंग मान जो वर्कशीट के नाम का प्रतिनिधित्व करता है। |
| range | WorksheetRange | वर्कशीट के आकार का प्रतिनिधित्व करने वाला [`WorksheetRange`](../../worksheetrange) क्लास का एक इंस्टेंस। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentOutOfRangeException | वर्कशीट का सूचकांक नकारात्मक नहीं हो सकता। |
| ArgumentNullException | वर्कशीट का आकार `null` नहीं हो सकता। |

### संबंधित देखें

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
