---
title: TemplateLinkedPosition
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Παρέχει μια θέση πεδίου προτύπου που χρησιμοποιεί το συνδεδεμένο πεδίο.
type: docs
weight: 700
url: /el/net/groupdocs.parser.templates/templatelinkedposition/
---
## TemplateLinkedPosition class

Παρέχει μια θέση πεδίου προτύπου που χρησιμοποιεί το συνδεδεμένο πεδίο.

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | Αρχικοποιεί μια νέα παρουσία του[`TemplateLinkedPosition`](../templatelinkedposition) τάξη. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | Αρχικοποιεί μια νέα παρουσία του[`TemplateLinkedPosition`](../templatelinkedposition) τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | Λαμβάνει την τιμή που υποδεικνύει εάν[`SearchArea`](./searcharea) κλιμακώνεται με το μέγεθος του συνδεδεμένου πεδίου. |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | Λαμβάνει τις άκρες του συνδεδεμένου πεδίου όπου γίνεται αναζήτηση ενός πεδίου. |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | Λαμβάνει το συνδεδεμένο όνομα πεδίου. |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | Λαμβάνει το μέγεθος της περιοχής όπου γίνεται αναζήτηση ενός πεδίου. |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει τον κωδικό για την κατάσταση εάν είναι γνωστό ότι το πεδίο με αριθμό τιμολογίου τοποθετείται στη δεξιά της συμβολοσειράς "Αριθμός τιμολογίου", χρησιμοποιείται ο ακόλουθος κωδικός:

```csharp
// Δημιουργήστε ένα πεδίο προτύπου regex για να βρείτε το κείμενο "Αριθμός Τιμολογίου".
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// Δημιουργήστε ένα σχετικό πεδίο προτύπου που σχετίζεται με το πεδίο "Τιμολόγιο" και εξαγάγετε την τιμή στα δεξιά του
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### Δείτε επίσης

* class [TemplatePosition](../templateposition)
* χώρος ονομάτων [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* συνέλευση [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
