---
title: "Parser"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Inizializza una nuova istanza della classe Parsergroupdocs.parser/parser per estrarre dati da un URI."
type: docs
weight: 10
url: /it/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un URI.

```csharp
public Parser(Uri uri)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| uri | Uri | L'URI a cui viene inviata la richiesta. |

### Vedi anche

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un URI con *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| uri | Uri | L'URI a cui viene inviata la richiesta. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |

### Vedi anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un URI con *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| uri | Uri | L'URI a cui viene inviata la richiesta. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Vedi anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un URI con *loadOptions* e *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| uri | Uri | L'URI a cui viene inviata la richiesta. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Vedi anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un database.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| connessione | DbConnection | La connessione al database. |

### Osservazioni

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Esempi

Il seguente esempio mostra come estrarre dati da un database Sqlite:

```csharp
// Crea l'oggetto DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crea un'istanza della classe Parser per estrarre le tabelle dal database
using (Parser parser = new Parser(connection))
{
    // Verifica se l'estrazione del testo è supportata
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Verifica se l'estrazione del toc è supportata
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Ottieni un elenco di tabelle
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itera sulle tabelle
    foreach (TocItem i in toc)
    {
        // Stampa il nome della tabella
        Console.WriteLine(i.Text);
        // Estrai il contenuto di una tabella come testo
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Vedi anche

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un database.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| connessione | DbConnection | La connessione al database. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Esempi

Il seguente esempio mostra come estrarre dati da un database Sqlite:

```csharp
// Crea l'oggetto DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crea un'istanza della classe Parser per estrarre le tabelle dal database
using (Parser parser = new Parser(connection))
{
    // Verifica se l'estrazione del testo è supportata
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Verifica se l'estrazione del toc è supportata
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Ottieni un elenco di tabelle
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itera sulle tabelle
    foreach (TocItem i in toc)
    {
        // Stampa il nome della tabella
        Console.WriteLine(i.Text);
        // Estrai il contenuto di una tabella come testo
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Vedi anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un server di posta elettronica remoto.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| connessione | EmailConnection | La connessione email. |

### Osservazioni

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Esempi

Il seguente esempio mostra come estrarre email da Exchange Server:

```csharp
// Crea l'oggetto di connessione per il protocollo Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crea un'istanza della classe Parser per estrarre email dal server remoto
using (Parser parser = new Parser(connection))
{
    // Verifica se l'estrazione del contenitore è supportata
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Estrai i messaggi email dal server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itera sugli allegati
    foreach (ContainerItem item in emails)
    {
        // Crea un'istanza della classe Parser per il messaggio email
        using (Parser emailParser = item.OpenParser())
        {
            // Estrai il testo dell'email
            using (TextReader reader = emailParser.GetText())
            {
                // Stampa il testo dell'email
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Vedi anche

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Inizializza una nuova istanza della classe [`Parser`](../../parser) per estrarre dati da un server di posta elettronica remoto.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| connessione | EmailConnection | La connessione email. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Esempi

Il seguente esempio mostra come estrarre email da Exchange Server:

```csharp
// Crea l'oggetto di connessione per il protocollo Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crea un'istanza della classe Parser per estrarre email dal server remoto
using (Parser parser = new Parser(connection))
{
    // Verifica se l'estrazione del contenitore è supportata
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Estrai i messaggi email dal server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itera sugli allegati
    foreach (ContainerItem item in emails)
    {
        // Crea un'istanza della classe Parser per il messaggio email
        using (Parser emailParser = item.OpenParser())
        {
            // Estrai il testo dell'email
            using (TextReader reader = emailParser.GetText())
            {
                // Stampa il testo dell'email
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Vedi anche

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Inizializza una nuova istanza della classe [`Parser`](../../parser).

```csharp
public Parser(string filePath)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| filePath | Stringa | Il percorso del file. |

### Osservazioni

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Esempi

Il seguente esempio mostra come caricare il documento dal disco locale:

```csharp
// Crea un'istanza della classe Parser con il filePath
using (Parser parser = new Parser(filePath))
{
    // Estrai un testo nel lettore
    using (TextReader reader = parser.GetText())
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, il lettore è null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Vedi anche

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Inizializza una nuova istanza della classe [`Parser`](../../parser) con [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| filePath | Stringa | Il percorso del file. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |

### Osservazioni

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Esempi

La password del documento è passata dalla classe LoadOptions:

```csharp
try
{
    // Crea un'istanza della classe Parser con la password:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Verifica se l'estrazione del testo è supportata
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Stampa il testo del documento
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Stampa il messaggio se la password è errata o vuota
    Console.WriteLine("Invalid password");
}
```

### Vedi anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Inizializza una nuova istanza della classe [`Parser`](../../parser) con [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| filePath | Stringa | Il percorso del file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Vedi anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Inizializza una nuova istanza della classe [`Parser`](../../parser) con [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) e [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| filePath | Stringa | Il percorso del file. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Esempi

Il seguente esempio mostra come ricevere le informazioni tramite l'interfaccia [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Crea un'istanza della classe Logger
    Logger logger = new Logger();
    // Crea un'istanza della classe Parser con le impostazioni del parser
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Verifica se l'estrazione del testo è supportata
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Stampa il testo del documento
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
        // Stampa il messaggio di errore
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Stampa il messaggio di evento
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Stampa il messaggio di avviso
        Console.WriteLine("Warning: " + message);
    }
}
```

### Vedi anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Inizializza una nuova istanza della classe [`Parser`](../../parser).

```csharp
public Parser(Stream document)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documento | Stream | Il flusso di input di origine. |

### Osservazioni

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Esempi

Il seguente esempio mostra come caricare il documento dallo stream:

```csharp
// Crea un'istanza della classe Parser con lo stream
using (Parser parser = new Parser(stream))
{
    // Estrai un testo nel lettore
    using (TextReader reader = parser.GetText())
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, il lettore è null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Vedi anche

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Inizializza una nuova istanza della classe [`Parser`](../../parser) con [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documento | Stream | Il flusso di input di origine. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |

### Osservazioni

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Esempi

In alcuni casi è necessario definire [`FileFormat`](../../../groupdocs.parser.options/fileformat). Sia per casi speciali (database, server di posta elettronica) sia per rilevare i tipi di file in base al contenuto:

```csharp
// Crea un'istanza della classe Parser per documento markdown
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Verifica se l'estrazione del testo è supportata
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Stampa il testo del documento
        // Il markdown è rilevato; il testo senza simboli speciali viene stampato
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

La password del documento è fornita dalla classe [`LoadOptions`](../../../groupdocs.parser.options/loadoptions):

```csharp
try
{
    // Crea un'istanza della classe Parser con la password:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Verifica se l'estrazione del testo è supportata
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Stampa il testo del documento
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Stampa il messaggio se la password è errata o vuota
    Console.WriteLine("Invalid password");
}
```

### Vedi anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Inizializza una nuova istanza della classe [`Parser`](../../parser) con [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documento | Stream | Il flusso di input di origine. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Vedi anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Inizializza una nuova istanza della classe [`Parser`](../../parser) con [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) e [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documento | Stream | Il flusso di input di origine. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Esempi

Il seguente esempio mostra come ricevere le informazioni tramite l'interfaccia [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Crea un'istanza della classe Logger
    Logger logger = new Logger();
    // Crea un'istanza della classe Parser con le impostazioni del parser
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Verifica se l'estrazione del testo è supportata
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Stampa il testo del documento
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
        // Stampa il messaggio di errore
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Stampa il messaggio di evento
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Stampa il messaggio di avviso
        Console.WriteLine("Warning: " + message);
    }
}
```

### Vedi anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
