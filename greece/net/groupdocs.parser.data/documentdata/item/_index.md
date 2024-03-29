---
title: Item
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Λαμβάνει τα δεδομένα πεδίου με ένα ευρετήριο.
type: docs
weight: 30
url: /el/net/groupdocs.parser.data/documentdata/item/
---
## DocumentData indexer

Λαμβάνει τα δεδομένα πεδίου με ένα ευρετήριο.

```csharp
public FieldData this[int index] { get; }
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| index | Ο μηδενικός δείκτης του πεδίου. |

### Επιστρεφόμενη Αξία

Ένα παράδειγμα του[`FieldData`](../../fielddata) τάξη.

### Παραδείγματα

Επανάληψη μέσω όλων των πεδίων:

[`FieldData`](../../fielddata) η κλάση αντιπροσωπεύει δεδομένα πεδίου. Ανάλογα με το πεδίο[`PageArea`](../../fielddata/pagearea) Το property μπορεί να περιέχει οποιονδήποτε από τους κληρονόμους του[`PageArea`](../../pagearea) τάξη. Για παράδειγμα,[`ParseForm`](../../../groupdocs.parser/parser/parseform) μέθοδος εξάγει μόνο πεδία κειμένου:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

```csharp
// Δημιουργία του αναλυτή
using (Parser parser = new Parser(filePath))
{
    // Εξαγωγή δεδομένων από τη φόρμα PDF
    DocumentData data = parser.ParseForm();
    // Επανάληψη σε εξαγόμενα πεδία
    for (int i = 0; i < data.Count; i++)
    {
        // Λήψη του εξαγόμενου πεδίου
        FieldData field = data[i];
        // Εκτυπώστε το όνομα του πεδίου
        Console.Write(field.Name + ": ");
        // Ελέγξτε αν η τιμή του πεδίου είναι κείμενο και εκτυπώστε το
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Δείτε επίσης

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* χώρος ονομάτων [GroupDocs.Parser.Data](../../documentdata)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
