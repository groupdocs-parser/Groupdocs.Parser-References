---
title: Features
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Obtiene las funciones admitidas.
type: docs
weight: 20
url: /es/net/groupdocs.parser/parser/features/
---
## Parser.Features property

Obtiene las funciones admitidas.

```csharp
public Features Features { get; }
```

### El valor de la propiedad

una instancia de[`Features`](../../../groupdocs.parser.options/features) clase que representa las funciones admitidas.

### Observaciones

**Aprende más:**

* [Obtener funciones compatibles](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### Ejemplos

Si la característica no es compatible, el método devuelve`nulo` en lugar del valor. Algunas operaciones pueden consumir mucho tiempo. Por lo tanto, no es óptimo llamar al método solo para comprobar la compatibilidad con la función. Para este propósito se utiliza la propiedad Features:

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

### Ver también

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->