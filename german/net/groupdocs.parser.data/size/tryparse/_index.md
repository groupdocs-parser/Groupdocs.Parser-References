---
title: "TryParse"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Konvertiert die Zeichenkettenrepräsentation einer Größe in das entsprechende Klassenobjekt. Ein Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist."
type: docs
weight: 70
url: /de/net/groupdocs.parser.data/size/tryparse/
---

## Size.TryParse method

Konvertiert die Zeichenkettenrepräsentation einer Größe in das entsprechende Klassenobjekt. Ein Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist.

```csharp
public static bool TryParse(string s, out Size size)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | String | Eine Zeichenkette, die eine Größe zum Konvertieren enthält. |
| size | Size& | Wenn die Methode zurückkehrt, enthält sie die Instanz der [`Size`](../../size)-Klasse, die dem im Parameter *s* angegebenen Wert entspricht, falls die Konvertierung erfolgreich war; andernfalls `null`. |

### Rückgabewert

`true`, wenn *s* erfolgreich konvertiert wird; andernfalls `false`.

### Siehe auch

* class [Size](../../size)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
