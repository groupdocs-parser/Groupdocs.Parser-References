---
title: TryParse
second_title: GroupDocs.Parser for .NET API Reference
description: Converts the string representation of a point to its class equivalent. A return value indicates whether the conversion is succeeded or failed.
type: docs
weight: 60
url: /net/groupdocs.parser.data/point/tryparse/
---
## Point.TryParse method

Converts the string representation of a point to its class equivalent. A return value indicates whether the conversion is succeeded or failed.

```csharp
public static bool TryParse(string s, out Point point)
```

| Parameter | Type | Description |
| --- | --- | --- |
| s | String | A string containing a point to convert. |
| point | Point& | When the method returns, it contains the instance of [`Point`](../../point) class that is equivalent to the value specified in *s* parameter, if the conversion is succeeded; otherwise, `null`. |

### Return Value

`true` if *s* is converted successfully; otherwise, `false`.

### See Also

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
