---
title: Parser
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Αρχικοποιεί μια νέα παρουσία τουParsergroupdocs.parser/parser κλάση για εξαγωγή δεδομένων από μια βάση δεδομένων.
type: docs
weight: 10
url: /el/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) κλάση για εξαγωγή δεδομένων από μια βάση δεδομένων.

```csharp
public Parser(DbConnection connection)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connection | DbConnection | Η σύνδεση της βάσης δεδομένων. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή δεδομένων από βάσεις δεδομένων](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε δεδομένα από τη βάση δεδομένων Sqlite:

```csharp
// Δημιουργία αντικειμένου DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Δημιουργήστε μια παρουσία κλάσης Parser για εξαγωγή πινάκων από τη βάση δεδομένων
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Ελέγξτε αν υποστηρίζεται η εξαγωγή toc
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Λήψη λίστας πινάκων
    IEnumerable<TocItem> toc = parser.GetToc();
    // Επανάληψη πάνω από πίνακες
    foreach (TocItem i in toc)
    {
        // Εκτυπώστε το όνομα του πίνακα
        Console.WriteLine(i.Text);
        // Εξαγωγή περιεχομένου πίνακα ως κείμενο
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) κλάση για εξαγωγή δεδομένων από μια βάση δεδομένων.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connection | DbConnection | Η σύνδεση της βάσης δεδομένων. |
| parserSettings | ParserSettings | Οι ρυθμίσεις ανάλυσης που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή δεδομένων από βάσεις δεδομένων](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Ξύλευση](https://docs.groupdocs.com/display/parsernet/Logging)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε δεδομένα από τη βάση δεδομένων Sqlite:

```csharp
// Δημιουργία αντικειμένου DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Δημιουργήστε μια παρουσία κλάσης Parser για εξαγωγή πινάκων από τη βάση δεδομένων
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Ελέγξτε αν υποστηρίζεται η εξαγωγή toc
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Λήψη λίστας πινάκων
    IEnumerable<TocItem> toc = parser.GetToc();
    // Επανάληψη πάνω από πίνακες
    foreach (TocItem i in toc)
    {
        // Εκτυπώστε το όνομα του πίνακα
        Console.WriteLine(i.Text);
        // Εξαγωγή περιεχομένου πίνακα ως κείμενο
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) κλάση για εξαγωγή δεδομένων από απομακρυσμένο διακομιστή email.

```csharp
public Parser(EmailConnection connection)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connection | EmailConnection | Η σύνδεση email. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή email από απομακρυσμένο διακομιστή μέσω πρωτοκόλλων POP, IMAP ή Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε μηνύματα ηλεκτρονικού ταχυδρομείου από τον Exchange Server:

```csharp
// Δημιουργήστε το αντικείμενο σύνδεσης για το πρωτόκολλο Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Δημιουργήστε μια παρουσία της κλάσης Parser για εξαγωγή μηνυμάτων ηλεκτρονικού ταχυδρομείου από τον απομακρυσμένο διακομιστή
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε εάν υποστηρίζεται η εξαγωγή κοντέινερ
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Εξαγωγή μηνυμάτων email από τον διακομιστή
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Επανάληψη σε συνημμένα
    foreach (ContainerItem item in emails)
    {
        // Δημιουργήστε μια παρουσία της κλάσης Parser για μήνυμα ηλεκτρονικού ταχυδρομείου
        using (Parser emailParser = item.OpenParser())
        {
            // Εξαγωγή του κειμένου email
            using (TextReader reader = emailParser.GetText())
            {
                // Εκτυπώστε το κείμενο του email
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Δείτε επίσης

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) κλάση για εξαγωγή δεδομένων από απομακρυσμένο διακομιστή email.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connection | EmailConnection | Η σύνδεση email. |
| parserSettings | ParserSettings | Οι ρυθμίσεις ανάλυσης που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή email από απομακρυσμένο διακομιστή μέσω πρωτοκόλλων POP, IMAP ή Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Ξύλευση](https://docs.groupdocs.com/display/parsernet/Logging)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε μηνύματα ηλεκτρονικού ταχυδρομείου από τον Exchange Server:

```csharp
// Δημιουργήστε το αντικείμενο σύνδεσης για το πρωτόκολλο Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Δημιουργήστε μια παρουσία της κλάσης Parser για εξαγωγή μηνυμάτων ηλεκτρονικού ταχυδρομείου από τον απομακρυσμένο διακομιστή
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε εάν υποστηρίζεται η εξαγωγή κοντέινερ
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Εξαγωγή μηνυμάτων email από τον διακομιστή
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Επανάληψη σε συνημμένα
    foreach (ContainerItem item in emails)
    {
        // Δημιουργήστε μια παρουσία της κλάσης Parser για μήνυμα ηλεκτρονικού ταχυδρομείου
        using (Parser emailParser = item.OpenParser())
        {
            // Εξαγωγή του κειμένου email
            using (TextReader reader = emailParser.GetText())
            {
                // Εκτυπώστε το κείμενο του email
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Δείτε επίσης

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη.

```csharp
public Parser(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Φόρτωση εγγράφου από τοπικό δίσκο](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να φορτώσετε το έγγραφο από τον τοπικό δίσκο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser με το filePath
using (Parser parser = new Parser(filePath))
{
    // Εξαγωγή κειμένου στον αναγνώστη
    using (TextReader reader = parser.GetText())
    {
        // Εκτύπωση κειμένου από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι μηδενικός
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη με[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Φόρτωση συγκεκριμένων μορφών αρχείων](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Φόρτωση εγγράφων που προστατεύονται με κωδικό πρόσβασης](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Φόρτωση εγγράφου από τοπικό δίσκο](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Παραδείγματα

Ο κωδικός πρόσβασης του εγγράφου μεταβιβάζεται από την κλάση LoadOptions:

```csharp
try
{
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τον κωδικό πρόσβασης:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Εκτυπώστε το κείμενο του εγγράφου
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Εκτυπώστε το μήνυμα εάν ο κωδικός πρόσβασης είναι λανθασμένος ή κενός
    Console.WriteLine("Invalid password");
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη με[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |
| parserSettings | ParserSettings | Οι ρυθμίσεις ανάλυσης που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Δείτε επίσης

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη με[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) και[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |
| parserSettings | ParserSettings | Οι ρυθμίσεις ανάλυσης που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Φόρτωση συγκεκριμένων μορφών αρχείων](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Φόρτωση εγγράφων που προστατεύονται με κωδικό πρόσβασης](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Ξύλευση](https://docs.groupdocs.com/display/parsernet/Logging)
* [Φόρτωση εγγράφου από τοπικό δίσκο](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να λαμβάνετε τις πληροφορίες μέσω[`ILogger`](../../../groupdocs.parser.options/ilogger) διεπαφή:

```csharp
// δοκιμάστε
{
    // Δημιουργήστε μια παρουσία της κλάσης Logger
    Logger logger = new Logger();
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τις ρυθμίσεις του parser
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Εκτυπώστε το κείμενο του εγγράφου
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Αγνοήστε την εξαίρεση
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Μήνυμα σφάλματος εκτύπωσης
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Εκτύπωση μηνύματος συμβάντος
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Εκτύπωση προειδοποιητικού μηνύματος
        Console.WriteLine("Warning: " + message);
    }
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη.

```csharp
public Parser(Stream document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Η ροή εισόδου της πηγής. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Φόρτωση εγγράφου από τη ροή](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να φορτώσετε το έγγραφο από τη ροή:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser με τη ροή
using (Parser parser = new Parser(stream))
{
    // Εξαγωγή κειμένου στον αναγνώστη
    using (TextReader reader = parser.GetText())
    {
        // Εκτύπωση κειμένου από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι μηδενικός
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη με[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Η ροή εισόδου της πηγής. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Φόρτωση συγκεκριμένων μορφών αρχείων](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Φόρτωση εγγράφων που προστατεύονται με κωδικό πρόσβασης](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Φόρτωση εγγράφου από τη ροή](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Παραδείγματα

Σε ορισμένες περιπτώσεις είναι απαραίτητο να οριστεί[`FileFormat`](../../../groupdocs.parser.options/fileformat). Τόσο για ειδικές περιπτώσεις (βάσεις δεδομένων, διακομιστής email) όσο και για τον εντοπισμό τύπων αρχείων με βάση το περιεχόμενο:

Ο κωδικός πρόσβασης του εγγράφου διαβιβάζεται[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) τάξη:

```csharp
// Δημιουργία μιας παρουσίας της κλάσης Parser για έγγραφο σήμανσης
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Εκτυπώστε το κείμενο του εγγράφου
        // Εντοπίζεται Markdown. εκτυπώνεται κείμενο χωρίς ειδικά σύμβολα
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τον κωδικό πρόσβασης:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Εκτυπώστε το κείμενο του εγγράφου
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Εκτυπώστε το μήνυμα εάν ο κωδικός πρόσβασης είναι λανθασμένος ή κενός
    Console.WriteLine("Invalid password");
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη με[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Η ροή εισόδου της πηγής. |
| parserSettings | ParserSettings | Οι ρυθμίσεις ανάλυσης που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Δείτε επίσης

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Αρχικοποιεί μια νέα παρουσία του[`Parser`](../../parser) τάξη με[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) και[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Η ροή εισόδου της πηγής. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |
| parserSettings | ParserSettings | Οι ρυθμίσεις ανάλυσης που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Φόρτωση συγκεκριμένων μορφών αρχείων](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Φόρτωση εγγράφων που προστατεύονται με κωδικό πρόσβασης](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Φόρτωση εγγράφου από τη ροή](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Ξύλευση](https://docs.groupdocs.com/display/parsernet/Logging)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να λαμβάνετε τις πληροφορίες μέσω[`ILogger`](../../../groupdocs.parser.options/ilogger) διεπαφή:

```csharp
// δοκιμάστε
{
    // Δημιουργήστε μια παρουσία της κλάσης Logger
    Logger logger = new Logger();
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τις ρυθμίσεις του parser
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Ελέγξτε αν υποστηρίζεται η εξαγωγή κειμένου
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Εκτυπώστε το κείμενο του εγγράφου
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Αγνοήστε την εξαίρεση
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Μήνυμα σφάλματος εκτύπωσης
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Εκτύπωση μηνύματος συμβάντος
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Εκτύπωση προειδοποιητικού μηνύματος
        Console.WriteLine("Warning: " + message);
    }
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
