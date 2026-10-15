---
title: "Αναλυτής"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αρχικοποιεί ένα νέο αντικείμενο της κλάσης Parsergroupdocs.parser/parser για να εξάγει δεδομένα από ένα URI."
type: docs
weight: 10
url: /el/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από ένα URI.

```csharp
public Parser(Uri uri)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| uri | Uri | Το Uri στο οποίο αποστέλλεται το αίτημα. |

### Δείτε επίσης

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από ένα URI με *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| uri | Uri | Το Uri στο οποίο αποστέλλεται το αίτημα. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από ένα URI με *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| uri | Uri | Το Uri στο οποίο αποστέλλεται το αίτημα. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Δείτε επίσης

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από ένα URI με *loadOptions* και *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| uri | Uri | Το Uri στο οποίο αποστέλλεται το αίτημα. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από μια βάση δεδομένων.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| σύνδεση | DbConnection | Η σύνδεση της βάσης δεδομένων. |

### Σχόλια

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε δεδομένα από τη βάση δεδομένων Sqlite:

```csharp
// Δημιουργία αντικειμένου DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Δημιουργία ενός αντικειμένου της κλάσης Parser για να εξάγετε πίνακες από τη βάση δεδομένων
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Ελέγξτε αν η εξαγωγή toc υποστηρίζεται
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Λήψη λίστας πινάκων
    IEnumerable<TocItem> toc = parser.GetToc();
    // Επανάληψη πάνω στους πίνακες
    foreach (TocItem i in toc)
    {
        // Εκτύπωση του ονόματος του πίνακα
        Console.WriteLine(i.Text);
        // Εξαγωγή του περιεχομένου του πίνακα ως κείμενο
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από μια βάση δεδομένων.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| σύνδεση | DbConnection | Η σύνδεση της βάσης δεδομένων. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Σχόλια

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε δεδομένα από τη βάση δεδομένων Sqlite:

```csharp
// Δημιουργία αντικειμένου DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Δημιουργία ενός αντικειμένου της κλάσης Parser για να εξάγετε πίνακες από τη βάση δεδομένων
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Ελέγξτε αν η εξαγωγή toc υποστηρίζεται
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Λήψη λίστας πινάκων
    IEnumerable<TocItem> toc = parser.GetToc();
    // Επανάληψη πάνω στους πίνακες
    foreach (TocItem i in toc)
    {
        // Εκτύπωση του ονόματος του πίνακα
        Console.WriteLine(i.Text);
        // Εξαγωγή του περιεχομένου του πίνακα ως κείμενο
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από έναν απομακρυσμένο διακομιστή email.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| σύνδεση | EmailConnection | Η σύνδεση email. |

### Σχόλια

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε email από τον Exchange Server:

```csharp
// Δημιουργία του αντικειμένου σύνδεσης για το πρωτόκολλο Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Δημιουργία ενός αντικειμένου της κλάσης Parser για να εξάγετε email από τον απομακρυσμένο διακομιστή
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε αν η εξαγωγή του container υποστηρίζεται
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Εξαγωγή μηνυμάτων email από τον διακομιστή
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Επανάληψη στα συνημμένα
    foreach (ContainerItem item in emails)
    {
        // Δημιουργήστε μια παρουσία της κλάσης Parser για το μήνυμα email
        using (Parser emailParser = item.OpenParser())
        {
            // Εξάγετε το κείμενο του email
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Parser`](../../parser) για να εξάγει δεδομένα από έναν απομακρυσμένο διακομιστή email.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| σύνδεση | EmailConnection | Η σύνδεση email. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Σχόλια

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε email από τον Exchange Server:

```csharp
// Δημιουργία του αντικειμένου σύνδεσης για το πρωτόκολλο Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Δημιουργία ενός αντικειμένου της κλάσης Parser για να εξάγετε email από τον απομακρυσμένο διακομιστή
using (Parser parser = new Parser(connection))
{
    // Ελέγξτε αν η εξαγωγή του container υποστηρίζεται
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Εξαγωγή μηνυμάτων email από τον διακομιστή
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Επανάληψη στα συνημμένα
    foreach (ContainerItem item in emails)
    {
        // Δημιουργήστε μια παρουσία της κλάσης Parser για το μήνυμα email
        using (Parser emailParser = item.OpenParser())
        {
            // Εξάγετε το κείμενο του email
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser).

```csharp
public Parser(string filePath)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |

### Σχόλια

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να φορτώσετε το έγγραφο από τον τοπικό δίσκο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser με το filePath
using (Parser parser = new Parser(filePath))
{
    // Εξάγετε κείμενο στον αναγνώστη
    using (TextReader reader = parser.GetText())
    {
        // Εκτυπώστε κείμενο από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser) με το [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |

### Σχόλια

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Παραδείγματα

Ο κωδικός πρόσβασης του εγγράφου περνιέται από την κλάση LoadOptions:

```csharp
try
{
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τον κωδικό πρόσβασης:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser) με το [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Δείτε επίσης

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser) με το [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) και το [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή προς το αρχείο. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Σχόλια

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε τις πληροφορίες μέσω της διεπαφής [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Δημιουργήστε μια παρουσία της κλάσης Logger
    Logger logger = new Logger();
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τις ρυθμίσεις του parser
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
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
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Εκτυπώστε το μήνυμα σφάλματος
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Εκτυπώστε το μήνυμα συμβάντος
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Εκτυπώστε το μήνυμα προειδοποίησης
        Console.WriteLine("Warning: " + message);
    }
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser).

```csharp
public Parser(Stream document)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η πηγή ροής εισόδου. |

### Σχόλια

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να φορτώσετε το έγγραφο από τη ροή:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser με τη ροή
using (Parser parser = new Parser(stream))
{
    // Εξάγετε κείμενο στον αναγνώστη
    using (TextReader reader = parser.GetText())
    {
        // Εκτυπώστε κείμενο από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser) με το [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η πηγή ροής εισόδου. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |

### Σχόλια

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Παραδείγματα

Σε ορισμένες περιπτώσεις είναι απαραίτητο να οριστεί το [`FileFormat`](../../../groupdocs.parser.options/fileformat). Τόσο για ειδικές περιπτώσεις (βάσεις δεδομένων, διακομιστής email) όσο και για την ανίχνευση τύπων αρχείων βάσει του περιεχομένου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser για έγγραφο markdown
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Εκτυπώστε το κείμενο του εγγράφου
        // Το Markdown εντοπίζεται· το κείμενο χωρίς ειδικά σύμβολα εκτυπώνεται
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

Ο κωδικός πρόσβασης του εγγράφου περνιέται από την κλάση [`LoadOptions`](../../../groupdocs.parser.options/loadoptions):

```csharp
try
{
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τον κωδικό πρόσβασης:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser) με το [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η πηγή ροής εισόδου. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Δείτε επίσης

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../../parser) με το [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) και το [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η πηγή ροής εισόδου. |
| loadOptions | LoadOptions | Οι επιλογές για το άνοιγμα του αρχείου. |
| parserSettings | ParserSettings | Οι ρυθμίσεις του parser που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |

### Σχόλια

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε τις πληροφορίες μέσω της διεπαφής [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Δημιουργήστε μια παρουσία της κλάσης Logger
    Logger logger = new Logger();
    // Δημιουργήστε μια παρουσία της κλάσης Parser με τις ρυθμίσεις του parser
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Ελέγξτε εάν η εξαγωγή κειμένου υποστηρίζεται
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
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Εκτυπώστε το μήνυμα σφάλματος
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Εκτυπώστε το μήνυμα συμβάντος
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Εκτυπώστε το μήνυμα προειδοποίησης
        Console.WriteLine("Warning: " + message);
    }
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
