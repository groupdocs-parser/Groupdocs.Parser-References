---
title: Parser
second_title: Riferimento API GroupDocs.Parser per .NET
description: Inizializza una nuova istanza diParsergroupdocs.parser/parser classe per estrarre i dati da un database.
type: docs
weight: 10
url: /it/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Inizializza una nuova istanza di[`Parser`](../../parser) classe per estrarre i dati da un database.

```csharp
public Parser(DbConnection connection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connection | DbConnection | La connessione al database. |

### Osservazioni

**Saperne di più:**

* [Estrarre i dati dai database](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Esempi

L'esempio seguente mostra come estrarre i dati dal database Sqlite:

```csharp
// Crea un oggetto DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crea un'istanza della classe Parser per estrarre le tabelle dal database
using (Parser parser = new Parser(connection))
{
    // Controlla se l'estrazione del testo è supportata
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Controlla se l'estrazione di toc è supportata
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

### Guarda anche

* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Inizializza una nuova istanza di[`Parser`](../../parser) classe per estrarre i dati da un database.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connection | DbConnection | La connessione al database. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Saperne di più:**

* [Estrarre i dati dai database](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Registrazione](https://docs.groupdocs.com/display/parsernet/Logging)

### Esempi

L'esempio seguente mostra come estrarre i dati dal database Sqlite:

```csharp
// Crea un oggetto DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crea un'istanza della classe Parser per estrarre le tabelle dal database
using (Parser parser = new Parser(connection))
{
    // Controlla se l'estrazione del testo è supportata
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Controlla se l'estrazione di toc è supportata
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

### Guarda anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Inizializza una nuova istanza di[`Parser`](../../parser) classe per estrarre i dati da un server di posta remoto.

```csharp
public Parser(EmailConnection connection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connection | EmailConnection | La connessione e-mail. |

### Osservazioni

**Saperne di più:**

* [Estrai le email dal server remoto tramite i protocolli POP, IMAP o Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Esempi

L'esempio seguente mostra come estrarre le email da Exchange Server:

```csharp
// Crea l'oggetto connessione per il protocollo Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crea un'istanza della classe Parser per estrarre le email dal server remoto
using (Parser parser = new Parser(connection))
{
    // Controlla se l'estrazione del contenitore è supportata
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Estrai i messaggi di posta elettronica dal server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itera sugli allegati
    foreach (ContainerItem item in emails)
    {
        // Crea un'istanza della classe Parser per il messaggio di posta elettronica
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

### Guarda anche

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Inizializza una nuova istanza di[`Parser`](../../parser) classe per estrarre i dati da un server di posta remoto.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connection | EmailConnection | La connessione e-mail. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Saperne di più:**

* [Estrai le email dal server remoto tramite i protocolli POP, IMAP o Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Registrazione](https://docs.groupdocs.com/display/parsernet/Logging)

### Esempi

L'esempio seguente mostra come estrarre le email da Exchange Server:

```csharp
// Crea l'oggetto connessione per il protocollo Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crea un'istanza della classe Parser per estrarre le email dal server remoto
using (Parser parser = new Parser(connection))
{
    // Controlla se l'estrazione del contenitore è supportata
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Estrai i messaggi di posta elettronica dal server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itera sugli allegati
    foreach (ContainerItem item in emails)
    {
        // Crea un'istanza della classe Parser per il messaggio di posta elettronica
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

### Guarda anche

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Inizializza una nuova istanza di[`Parser`](../../parser) classe.

```csharp
public Parser(string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |

### Osservazioni

**Saperne di più:**

* [Carica il documento dal disco locale](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Esempi

L'esempio seguente mostra come caricare il documento dal disco locale:

```csharp
// Crea un'istanza della classe Parser con filePath
using (Parser parser = new Parser(filePath))
{
    // Estrai un testo nel lettore
    using (TextReader reader = parser.GetText())
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, un lettore è nullo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Guarda anche

* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Inizializza una nuova istanza di[`Parser`](../../parser) classe con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |

### Osservazioni

**Saperne di più:**

* [Caricamento di formati di file specifici](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Caricamento di documenti protetti da password](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Carica il documento dal disco locale](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Esempi

La password del documento viene passata dalla classe LoadOptions:

```csharp
try
{
    // Crea un'istanza della classe Parser con la password:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Controlla se l'estrazione del testo è supportata
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

### Guarda anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Inizializza una nuova istanza di[`Parser`](../../parser) classe con[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Guarda anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Inizializza una nuova istanza di[`Parser`](../../parser) classe con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) e[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Saperne di più:**

* [Caricamento di formati di file specifici](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Caricamento di documenti protetti da password](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Registrazione](https://docs.groupdocs.com/display/parsernet/Logging)
* [Carica il documento dal disco locale](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Esempi

L'esempio seguente mostra come ricevere le informazioni tramite[`ILogger`](../../../groupdocs.parser.options/ilogger) interfaccia:

```csharp
// Tentativo
{
    // Crea un'istanza della classe Logger
    Logger logger = new Logger();
    // Crea un'istanza della classe Parser con le impostazioni del parser
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Controlla se l'estrazione del testo è supportata
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
    ; // Ignora l'eccezione
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Stampa messaggio di errore
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Stampa il messaggio dell'evento
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Stampa il messaggio di avviso
        Console.WriteLine("Warning: " + message);
    }
}
```

### Guarda anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Inizializza una nuova istanza di[`Parser`](../../parser) classe.

```csharp
public Parser(Stream document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Il flusso di input di origine. |

### Osservazioni

**Saperne di più:**

* [Carica il documento dal flusso](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Esempi

L'esempio seguente mostra come caricare il documento dallo stream:

```csharp
// Crea un'istanza della classe Parser con lo stream
using (Parser parser = new Parser(stream))
{
    // Estrai un testo nel lettore
    using (TextReader reader = parser.GetText())
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, un lettore è nullo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Guarda anche

* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Inizializza una nuova istanza di[`Parser`](../../parser) classe con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Il flusso di input di origine. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |

### Osservazioni

**Saperne di più:**

* [Caricamento di formati di file specifici](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Caricamento di documenti protetti da password](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Carica il documento dal flusso](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Esempi

In alcuni casi è necessario definire[`FileFormat`](../../../groupdocs.parser.options/fileformat). Sia per casi speciali (database, server di posta elettronica) sia per rilevare i tipi di file in base al contenuto:

La password del documento viene trasmessa[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) classe:

```csharp
// Crea un'istanza della classe Parser per il documento markdown
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Controlla se l'estrazione del testo è supportata
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Stampa il testo del documento
        // Markdown viene rilevato; viene stampato il testo senza simboli speciali
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Crea un'istanza della classe Parser con la password:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Controlla se l'estrazione del testo è supportata
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

### Guarda anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Inizializza una nuova istanza di[`Parser`](../../parser) classe con[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Il flusso di input di origine. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Guarda anche

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Inizializza una nuova istanza di[`Parser`](../../parser) classe con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) e[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Il flusso di input di origine. |
| loadOptions | LoadOptions | Le opzioni per aprire il file. |
| parserSettings | ParserSettings | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |

### Osservazioni

**Saperne di più:**

* [Caricamento di formati di file specifici](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Caricamento di documenti protetti da password](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Carica il documento dal flusso](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Registrazione](https://docs.groupdocs.com/display/parsernet/Logging)

### Esempi

L'esempio seguente mostra come ricevere le informazioni tramite[`ILogger`](../../../groupdocs.parser.options/ilogger) interfaccia:

```csharp
// Tentativo
{
    // Crea un'istanza della classe Logger
    Logger logger = new Logger();
    // Crea un'istanza della classe Parser con le impostazioni del parser
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Controlla se l'estrazione del testo è supportata
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
    ; // Ignora l'eccezione
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Stampa messaggio di errore
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Stampa il messaggio dell'evento
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Stampa il messaggio di avviso
        Console.WriteLine("Warning: " + message);
    }
}
```

### Guarda anche

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
