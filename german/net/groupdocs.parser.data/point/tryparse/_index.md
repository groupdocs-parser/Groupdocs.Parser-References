---
title: "TryParse"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Konvertiert die Zeichenkettenrepräsentation eines Punktes in das entsprechende Klassenobjekt. Der Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist."
type: docs
weight: 80
url: /de/net/groupdocs.parser.data/point/tryparse/
---

## Point.TryParse method

Konvertiert die Zeichenkettenrepräsentation eines Punktes in das entsprechende Klassenobjekt. Der Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist.

```csharp
public static bool TryParse(string s, out Point point)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | String | Eine Zeichenkette, die einen Punkt zum Konvertieren enthält. |
| point | Point& | Wenn die Methode zurückkehrt, enthält sie die Instanz der Klasse [`Point`](../../point), die dem im Parameter *s* angegebenen Wert entspricht, falls die Konvertierung erfolgreich war; andernfalls `null`. |

### Rückgabewert

`true`, wenn *s* erfolgreich konvertiert wird; andernfalls `false`.

### Siehe auch

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
