---
title: Item
second_title: Riferimento API GroupDocs.Parser per .NET
description: Ottiene i dati del campo tramite un indice.
type: docs
weight: 30
url: /it/net/groupdocs.parser.data/documentdata/item/
---
## DocumentData indexer

Ottiene i dati del campo tramite un indice.

```csharp
public FieldData this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| index | L'indice in base zero del campo. |

### Valore di ritorno

Un'istanza di[`FieldData`](../../fielddata) classe.

### Esempi

Iterazione tramite tutti i campi:

[`FieldData`](../../fielddata) la classe rappresenta i dati del campo. A seconda del campo[`PageArea`](../../fielddata/pagearea) property può contenere qualsiasi erede di[`PageArea`](../../pagearea) classe. Per esempio,[`ParseForm`](../../../groupdocs.parser/parser/parseform) method estrae solo i campi di testo:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

```csharp
// Crea il parser
using (Parser parser = new Parser(filePath))
{
    // Estrai i dati dal modulo PDF
    DocumentData data = parser.ParseForm();
    // Itera sui campi estratti
    for (int i = 0; i < data.Count; i++)
    {
        // Ottieni il campo estratto
        FieldData field = data[i];
        // Stampa il nome del campo
        Console.Write(field.Name + ": ");
        // Controlla se il valore del campo è un testo e stampalo
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Guarda anche

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* spazio dei nomi [GroupDocs.Parser.Data](../../documentdata)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->