---
title: "TemplateTable"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης TemplateTablegroupdocs.parser.templates/templatetable με το όνομα σε ΚΕΦΑΛΑΙΑ."
type: docs
weight: 10
url: /el/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TemplateTable`](../../templatetable) με το όνομα σε ΚΕΦΑΛΑΙΑ.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| layout | TemplateTableLayout | Η διάταξη του πίνακα. |
| όνομα | String | Το όνομα του πίνακα. |

### Παραδείγματα

Ο πίνακας προτύπου ορίζεται από τη διάταξη του πίνακα εάν ο πίνακας δεν μπορεί να εντοπιστεί αυτόματα:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Δημιουργία προτύπου εγγράφου
Template template = new Template(new TemplateItem[] { table });
```

### Δείτε επίσης

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TemplateTable`](../../templatetable) με το όνομα σε ΚΕΦΑΛΑΙΑ.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| layout | TemplateTableLayout | Η διάταξη του πίνακα. |
| όνομα | String | Το όνομα του πίνακα. |
| pageWidth | Nullable`1 | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |

### Παραδείγματα

Ο πίνακας προτύπου ορίζεται από τη διάταξη του πίνακα εάν ο πίνακας δεν μπορεί να εντοπιστεί αυτόματα:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Δημιουργία προτύπου εγγράφου
Template template = new Template(new TemplateItem[] { table });
```

### Δείτε επίσης

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| layout | TemplateTableLayout | Η διάταξη του πίνακα. |
| όνομα | String | Το όνομα του πίνακα. |
| pageWidth | Nullable`1 | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
| useUpperCaseName | Boolean | Η τιμή που υποδεικνύει εάν ένα `name` μετατρέπεται σε ΚΕΦΑΛΑΙΑ. |

### Παραδείγματα

Ο πίνακας προτύπου ορίζεται από τη διάταξη του πίνακα εάν ο πίνακας δεν μπορεί να εντοπιστεί αυτόματα:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Δημιουργία προτύπου εγγράφου
Template template = new Template(new TemplateItem[] { table });
```

### Δείτε επίσης

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| παράμετροι | TemplateTableParameters | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
| όνομα | String | Το όνομα του πίνακα. |

### Παραδείγματα

Εάν ένας πίνακας προτύπου ορίζεται από τις παραμέτρους του ανιχνευτή, ο πίνακας ανιχνεύεται αυτόματα:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Δημιουργία προτύπου εγγράφου
Template template = new Template(new TemplateItem[] { table });
```

### Δείτε επίσης

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| παράμετροι | TemplateTableParameters | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
| όνομα | String | Το όνομα του πίνακα. |
| pageWidth | Nullable`1 | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |

### Παραδείγματα

Εάν ένας πίνακας προτύπου ορίζεται από τις παραμέτρους του ανιχνευτή, ο πίνακας ανιχνεύεται αυτόματα:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Δημιουργία προτύπου εγγράφου
Template template = new Template(new TemplateItem[] { table });
```

### Δείτε επίσης

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| παράμετροι | TemplateTableParameters | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
| όνομα | String | Το όνομα του πίνακα. |
| pageWidth | Nullable`1 | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
| useUpperCaseName | Boolean | Η τιμή που υποδεικνύει εάν ένα `name` μετατρέπεται σε ΚΕΦΑΛΑΙΑ. |

### Παραδείγματα

Εάν ένας πίνακας προτύπου ορίζεται από τις παραμέτρους του ανιχνευτή, ο πίνακας ανιχνεύεται αυτόματα:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Δημιουργία προτύπου εγγράφου
Template template = new Template(new TemplateItem[] { table });
```

### Δείτε επίσης

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
