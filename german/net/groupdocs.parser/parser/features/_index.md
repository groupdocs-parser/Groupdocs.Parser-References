---
title: "Funktionen"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Ruft die unterstützten Funktionen ab."
type: docs
weight: 20
url: /de/net/groupdocs.parser/parser/features/
---

## Parser.Features property

Ruft die unterstützten Funktionen ab.

```csharp
public Features Features { get; }
```

### Property Value

Eine Instanz der [`Features`](../../../groupdocs.parser.options/features)-Klasse, die die unterstützten Funktionen darstellt.

### Hinweise

**Learn more:**

* [Get supported features](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### Beispiele

Wenn die Funktion nicht unterstützt wird, gibt die Methode `null` anstelle des Wertes zurück. Einige Vorgänge können erheblichen Zeitaufwand erfordern. Daher ist es nicht optimal, die Methode nur zum Prüfen der Unterstützung der Funktion aufzurufen. Zu diesem Zweck wird die Eigenschaft Features verwendet:

```csharp
using(Parser parser = new Parser("doc.zip"))
{
    if(!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported");
        return;
    }
 
    using(TextReader reader = parser.GetText())
    {
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
