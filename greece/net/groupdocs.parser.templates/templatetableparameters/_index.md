---
title: TemplateTableParameters
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Παρέχει παραμέτρους για τους αλγόριθμους ανίχνευσης πινάκων.
type: docs
weight: 760
url: /el/net/groupdocs.parser.templates/templatetableparameters/
---
## TemplateTableParameters class

Παρέχει παραμέτρους για τους αλγόριθμους ανίχνευσης πινάκων.

```csharp
public sealed class TemplateTableParameters
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Αρχικοποιεί μια νέα παρουσία του[`TemplateTableParameters`](../templatetableparameters) τάξη. |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Αρχικοποιεί μια νέα παρουσία του[`TemplateTableParameters`](../templatetableparameters) τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Λαμβάνει την τιμή που υποδεικνύει εάν ο πίνακας έχει συγχωνευμένα κελιά. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Λαμβάνει τον ελάχιστο αριθμό στηλών του πίνακα. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Λαμβάνει τον ελάχιστο αριθμό σειρών του πίνακα. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Λαμβάνει το ελάχιστο διάστημα μεταξύ των στηλών του πίνακα. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Παίρνει την ορθογώνια περιοχή που περιέχει τον πίνακα. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Λαμβάνει τα διαχωριστικά στηλών του πίνακα. |

### Παρατηρήσεις

Υπάρχουν δύο αλγόριθμοι για την ανίχνευση ενός πίνακα:

* Επιτρέπει την ανίχνευση ενός πίνακα στην ορθογώνια περιοχή με στήλες συνόλου. Αυτός ο αλγόριθμος είναι χρήσιμος για απλούς πίνακες (χωρίς συγχωνευμένες στήλες) και παρέχει πιο ακριβή εντοπισμό.
* Επιτρέπει την ανίχνευση πίνακα σε οποιοδήποτε σημείο της σελίδας. Αυτός είναι ένας πιο περίπλοκος αλγόριθμος. Μπορεί να ανιχνεύσει πίνακες σε οποιοδήποτε σημείο της σελίδας. Πρόσθετες παράμετροι βοηθούν στον πιο σωστό εντοπισμό ενός πίνακα.

Σε ορισμένες περιπτώσεις, όταν οι αλγόριθμοι δεν μπορούν να εντοπίσουν έναν πίνακα ή να το κάνουν με μη ακριβή τρόπο [`TemplateTableLayout`](../templatetablelayout) χρησιμοποιείται κλάση.

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* συνέλευση [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->