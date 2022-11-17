---
title: Parser
second_title: GroupDocs.Parser för .NET API-referens
description: Initierar en ny instans avParsergroupdocs.parser/parser klass för att extrahera data från en databas.
type: docs
weight: 10
url: /sv/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Initierar en ny instans av[`Parser`](../../parser) klass för att extrahera data från en databas.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connection | DbConnection | Databasanslutningen. |

### Anmärkningar

**Läs mer:**

* [Extrahera data från databaser](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Exempel

Följande exempel visar hur man extraherar data från Sqlite-databasen:

```csharp
// Skapa DbConnection-objekt
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Skapa en instans av klassen Parser för att extrahera tabeller från databasen
using (Parser parser = new Parser(connection))
{
    // Kontrollera om textextraktion stöds
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Kontrollera om toc-extraktion stöds
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Få en lista med tabeller
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iterera över tabeller
    foreach (TocItem i in toc)
    {
        // Skriv ut tabellnamnet
        Console.WriteLine(i.Text);
        // Extrahera ett tabellinnehåll som en text
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Se även

* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initierar en ny instans av[`Parser`](../../parser) klass för att extrahera data från en databas.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connection | DbConnection | Databasanslutningen. |
| parserSettings | ParserSettings | Parserinställningarna som används för att anpassa dataextraktion. |

### Anmärkningar

**Läs mer:**

* [Extrahera data från databaser](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Skogsavverkning](https://docs.groupdocs.com/display/parsernet/Logging)

### Exempel

Följande exempel visar hur man extraherar data från Sqlite-databasen:

```csharp
// Skapa DbConnection-objekt
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Skapa en instans av klassen Parser för att extrahera tabeller från databasen
using (Parser parser = new Parser(connection))
{
    // Kontrollera om textextraktion stöds
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Kontrollera om toc-extraktion stöds
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Få en lista med tabeller
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iterera över tabeller
    foreach (TocItem i in toc)
    {
        // Skriv ut tabellnamnet
        Console.WriteLine(i.Text);
        // Extrahera ett tabellinnehåll som en text
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Se även

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initierar en ny instans av[`Parser`](../../parser) klass för att extrahera data från en fjärransluten e-postserver.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connection | EmailConnection | E-postanslutningen. |

### Anmärkningar

**Läs mer:**

* [Extrahera e-postmeddelanden från fjärrservern via POP-, IMAP- eller Exchange Web Services-protokoll](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Exempel

Följande exempel visar hur man extraherar e-postmeddelanden från Exchange Server:

```csharp
// Skapa anslutningsobjektet för Exchange Web Services-protokollet 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Skapa en instans av Parser-klassen för att extrahera e-postmeddelanden från fjärrservern
using (Parser parser = new Parser(connection))
{
    // Kontrollera om containerextraktion stöds
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extrahera e-postmeddelanden från servern
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Iterera över bilagor
    foreach (ContainerItem item in emails)
    {
        // Skapa en instans av Parser-klassen för e-postmeddelande
        using (Parser emailParser = item.OpenParser())
        {
            // Extrahera e-posttexten
            using (TextReader reader = emailParser.GetText())
            {
                // Skriv ut e-posttexten
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Se även

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initierar en ny instans av[`Parser`](../../parser) klass för att extrahera data från en fjärransluten e-postserver.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connection | EmailConnection | E-postanslutningen. |
| parserSettings | ParserSettings | Parserinställningarna som används för att anpassa dataextraktion. |

### Anmärkningar

**Läs mer:**

* [Extrahera e-postmeddelanden från fjärrservern via POP-, IMAP- eller Exchange Web Services-protokoll](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Skogsavverkning](https://docs.groupdocs.com/display/parsernet/Logging)

### Exempel

Följande exempel visar hur man extraherar e-postmeddelanden från Exchange Server:

```csharp
// Skapa anslutningsobjektet för Exchange Web Services-protokollet 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Skapa en instans av Parser-klassen för att extrahera e-postmeddelanden från fjärrservern
using (Parser parser = new Parser(connection))
{
    // Kontrollera om containerextraktion stöds
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extrahera e-postmeddelanden från servern
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Iterera över bilagor
    foreach (ContainerItem item in emails)
    {
        // Skapa en instans av Parser-klassen för e-postmeddelande
        using (Parser emailParser = item.OpenParser())
        {
            // Extrahera e-posttexten
            using (TextReader reader = emailParser.GetText())
            {
                // Skriv ut e-posttexten
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Se även

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_7}

Initierar en ny instans av[`Parser`](../../parser) class.

```csharp
public Parser(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökvägen till filen. |

### Anmärkningar

**Läs mer:**

* [Ladda dokument från lokal disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exempel

Följande exempel visar hur du laddar dokumentet från den lokala disken:

```csharp
// Skapa en instans av Parser-klassen med filsökvägen
using (Parser parser = new Parser(filePath))
{
    // Extrahera en text i läsaren
    using (TextReader reader = parser.GetText())
    {
        // Skriv ut en text från dokumentet
        // Om textextraktion inte stöds är en läsare null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Se även

* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_8}

Initierar en ny instans av[`Parser`](../../parser) klass med[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökvägen till filen. |
| loadOptions | LoadOptions | Alternativen för att öppna filen. |

### Anmärkningar

**Läs mer:**

* [Laddar specifika filformat](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Laddar lösenordsskyddade dokument](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Ladda dokument från lokal disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exempel

Dokumentlösenordet skickas av LoadOptions-klassen:

```csharp
try
{
    // Skapa en instans av Parser-klassen med lösenordet:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Kontrollera om textextraktion stöds
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Skriv ut dokumenttexten
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Skriv ut meddelandet om lösenordet är felaktigt eller tomt
    Console.WriteLine("Invalid password");
}
```

### Se även

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_9}

Initierar en ny instans av[`Parser`](../../parser) klass med[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) och[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökvägen till filen. |
| loadOptions | LoadOptions | Alternativen för att öppna filen. |
| parserSettings | ParserSettings | Parserinställningarna som används för att anpassa dataextraktion. |

### Anmärkningar

**Läs mer:**

* [Laddar specifika filformat](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Laddar lösenordsskyddade dokument](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Skogsavverkning](https://docs.groupdocs.com/display/parsernet/Logging)
* [Ladda dokument från lokal disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exempel

Följande exempel visar hur du tar emot informationen via[`ILogger`](../../../groupdocs.parser.options/ilogger) gränssnitt:

```csharp
// Prova
{
    // Skapa en instans av Logger-klassen
    Logger logger = new Logger();
    // Skapa en instans av Parser-klassen med parserinställningarna
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Kontrollera om textextraktion stöds
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Skriv ut dokumenttexten
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignorera undantaget
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Skriv ut felmeddelande
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Skriv ut händelsemeddelande
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Skriv ut varningsmeddelande
        Console.WriteLine("Warning: " + message);
    }
}
```

### Se även

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initierar en ny instans av[`Parser`](../../parser) class.

```csharp
public Parser(Stream document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | Stream | Källindataströmmen. |

### Anmärkningar

**Läs mer:**

* [Ladda dokument från stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Exempel

Följande exempel visar hur du laddar dokumentet från strömmen:

```csharp
// Skapa en instans av Parser-klassen med strömmen
using (Parser parser = new Parser(stream))
{
    // Extrahera en text i läsaren
    using (TextReader reader = parser.GetText())
    {
        // Skriv ut en text från dokumentet
        // Om textextraktion inte stöds är en läsare null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Se även

* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initierar en ny instans av[`Parser`](../../parser) klass med[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | Stream | Källindataströmmen. |
| loadOptions | LoadOptions | Alternativen för att öppna filen. |

### Anmärkningar

**Läs mer:**

* [Laddar specifika filformat](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Laddar lösenordsskyddade dokument](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Ladda dokument från stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Exempel

I vissa fall är det nödvändigt att definiera[`FileFormat`](../../../groupdocs.parser.options/fileformat). Både för specialfall (databaser, e-postserver) och för att upptäcka filtyper efter innehållet:

Dokumentlösenordet skickas förbi[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) klass:

```csharp
// Skapa en instans av Parser-klassen för markdown-dokument
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Kontrollera om textextraktion stöds
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Skriv ut dokumenttexten
        // Markdown har upptäckts; text utan speciella symboler skrivs ut
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Skapa en instans av Parser-klassen med lösenordet:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Kontrollera om textextraktion stöds
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Skriv ut dokumenttexten
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Skriv ut meddelandet om lösenordet är felaktigt eller tomt
    Console.WriteLine("Invalid password");
}
```

### Se även

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initierar en ny instans av[`Parser`](../../parser) klass med[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) och[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | Stream | Källindataströmmen. |
| loadOptions | LoadOptions | Alternativen för att öppna filen. |
| parserSettings | ParserSettings | Parserinställningarna som används för att anpassa dataextraktion. |

### Anmärkningar

**Läs mer:**

* [Laddar specifika filformat](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Laddar lösenordsskyddade dokument](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Ladda dokument från stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Skogsavverkning](https://docs.groupdocs.com/display/parsernet/Logging)

### Exempel

Följande exempel visar hur du tar emot informationen via[`ILogger`](../../../groupdocs.parser.options/ilogger) gränssnitt:

```csharp
// Prova
{
    // Skapa en instans av Logger-klassen
    Logger logger = new Logger();
    // Skapa en instans av Parser-klassen med parserinställningarna
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Kontrollera om textextraktion stöds
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Skriv ut dokumenttexten
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignorera undantaget
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Skriv ut felmeddelande
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Skriv ut händelsemeddelande
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Skriv ut varningsmeddelande
        Console.WriteLine("Warning: " + message);
    }
}
```

### Se även

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
