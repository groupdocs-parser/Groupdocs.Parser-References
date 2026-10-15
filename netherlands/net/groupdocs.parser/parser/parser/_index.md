---
title: "Parser"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Initialiseert een nieuw exemplaar van de Parsergroupdocs.parser/parser-klasse om gegevens uit een URI te extraheren."
type: docs
weight: 10
url: /nl/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens uit een URI te extraheren.

```csharp
public Parser(Uri uri)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uri | Uri | De Uri waar het verzoek naartoe wordt gestuurd. |

### Zie ook

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens uit een URI te extraheren met *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uri | Uri | De Uri waar het verzoek naartoe wordt gestuurd. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens uit een URI te extraheren met *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uri | Uri | De Uri waar het verzoek naartoe wordt gestuurd. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Zie ook

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens uit een URI te extraheren met *loadOptions* en *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uri | Uri | De Uri waar het verzoek naartoe wordt gestuurd. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens uit een database te extraheren.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| verbinding | DbConnection | De databaseverbinding. |

### Opmerkingen

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u gegevens uit een Sqlite-database kunt extraheren:

```csharp
// Maak DbConnection-object aan
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Maak een instantie van de Parser-klasse aan om tabellen uit de database te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleer of tekstextractie wordt ondersteund
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Controleren of toc-extractie wordt ondersteund
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Haal een lijst met tabellen op
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itereer over tabellen
    foreach (TocItem i in toc)
    {
        // Print de tabelnaam
        Console.WriteLine(i.Text);
        // Extraheer de inhoud van een tabel als tekst
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens uit een database te extraheren.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| verbinding | DbConnection | De databaseverbinding. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u gegevens uit een Sqlite-database kunt extraheren:

```csharp
// Maak DbConnection-object aan
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Maak een instantie van de Parser-klasse aan om tabellen uit de database te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleer of tekstextractie wordt ondersteund
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Controleren of toc-extractie wordt ondersteund
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Haal een lijst met tabellen op
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itereer over tabellen
    foreach (TocItem i in toc)
    {
        // Print de tabelnaam
        Console.WriteLine(i.Text);
        // Extraheer de inhoud van een tabel als tekst
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens van een externe e-mailserver te extraheren.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| verbinding | EmailConnection | De e-mailverbinding. |

### Opmerkingen

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u e-mails van Exchange Server kunt extraheren:

```csharp
// Maak het verbindingsobject aan voor het Exchange Web Services-protocol
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Maak een instantie van de Parser-klasse aan om e-mails van de externe server te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleren of containerextractie wordt ondersteund
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraheer e-mailberichten van de server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itereren over bijlagen
    foreach (ContainerItem item in emails)
    {
        // Maak een instantie van de Parser-klasse voor e‑mailbericht
        using (Parser emailParser = item.OpenParser())
        {
            // Extraheer de e‑mailtekst
            using (TextReader reader = emailParser.GetText())
            {
                // Print de e‑mailtekst
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Zie ook

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`Parser`](../../parser) klasse om gegevens van een externe e-mailserver te extraheren.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| verbinding | EmailConnection | De e-mailverbinding. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u e-mails van Exchange Server kunt extraheren:

```csharp
// Maak het verbindingsobject aan voor het Exchange Web Services-protocol
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Maak een instantie van de Parser-klasse aan om e-mails van de externe server te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleren of containerextractie wordt ondersteund
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraheer e-mailberichten van de server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itereren over bijlagen
    foreach (ContainerItem item in emails)
    {
        // Maak een instantie van de Parser-klasse voor e‑mailbericht
        using (Parser emailParser = item.OpenParser())
        {
            // Extraheer de e‑mailtekst
            using (TextReader reader = emailParser.GetText())
            {
                // Print de e‑mailtekst
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Zie ook

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse.

```csharp
public Parser(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |

### Opmerkingen

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Voorbeelden

Het volgende voorbeeld toont hoe het document van de lokale schijf te laden:

```csharp
// Maak een instantie van de Parser-klasse met het bestandspad
using (Parser parser = new Parser(filePath))
{
    // Extraheer een tekst naar de reader
    using (TextReader reader = parser.GetText())
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een reader `null`
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse met [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |

### Opmerkingen

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Voorbeelden

Het documentwachtwoord wordt door de LoadOptions-klasse doorgegeven:

```csharp
try
{
    // Maak een instantie van de Parser-klasse met het wachtwoord:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Controleer of tekstextractie wordt ondersteund
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print de documenttekst
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Print het bericht als het wachtwoord onjuist of leeg is
    Console.WriteLine("Invalid password");
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse met [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Zie ook

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse met [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) en [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Voorbeelden

Het volgende voorbeeld toont hoe de informatie via de [`ILogger`](../../../groupdocs.parser.options/ilogger)-interface te ontvangen:

```csharp
// probeer
{
    // Maak een instantie van de Logger-klasse
    Logger logger = new Logger();
    // Maak een instantie van de Parser-klasse met de parserinstellingen
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Controleer of tekstextractie wordt ondersteund
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print de documenttekst
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
        // Print foutmelding
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Print gebeurtenisbericht
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Print waarschuwingsbericht
        Console.WriteLine("Warning: " + message);
    }
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse.

```csharp
public Parser(Stream document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |

### Opmerkingen

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Voorbeelden

Het volgende voorbeeld toont hoe het document uit de stream te laden:

```csharp
// Maak een instantie van de Parser-klasse met de stream
using (Parser parser = new Parser(stream))
{
    // Extraheer een tekst naar de reader
    using (TextReader reader = parser.GetText())
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een reader `null`
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse met [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |

### Opmerkingen

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Voorbeelden

In sommige gevallen is het nodig om [`FileFormat`](../../../groupdocs.parser.options/fileformat) te definiëren. Zowel voor speciale gevallen (databases, e‑mailserver) als voor het detecteren van bestandstypen op basis van de inhoud:

```csharp
// Maak een instantie van de Parser-klasse voor een markdown-document
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Controleer of tekstextractie wordt ondersteund
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Print de documenttekst
        // Markdown wordt gedetecteerd; tekst zonder speciale symbolen wordt afgedrukt
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

Het documentwachtwoord wordt door de [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) klasse doorgegeven:

```csharp
try
{
    // Maak een instantie van de Parser-klasse met het wachtwoord:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Controleer of tekstextractie wordt ondersteund
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print de documenttekst
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Print het bericht als het wachtwoord onjuist of leeg is
    Console.WriteLine("Invalid password");
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse met [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Zie ook

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initialiseert een nieuwe instantie van de [`Parser`](../../parser)-klasse met [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) en [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Voorbeelden

Het volgende voorbeeld toont hoe de informatie via de [`ILogger`](../../../groupdocs.parser.options/ilogger)-interface te ontvangen:

```csharp
// probeer
{
    // Maak een instantie van de Logger-klasse
    Logger logger = new Logger();
    // Maak een instantie van de Parser-klasse met de parserinstellingen
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Controleer of tekstextractie wordt ondersteund
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print de documenttekst
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
        // Print foutmelding
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Print gebeurtenisbericht
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Print waarschuwingsbericht
        Console.WriteLine("Warning: " + message);
    }
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
