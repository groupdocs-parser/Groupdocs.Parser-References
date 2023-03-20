---
title: Parser
second_title: GroupDocs.Parser voor .NET API-referentie
description: Initialiseert een nieuw exemplaar van hetParsergroupdocs.parser/parser klasse om gegevens uit een database te extraheren.
type: docs
weight: 10
url: /nl/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klasse om gegevens uit een database te extraheren.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connection | DbConnection | De databaseverbinding. |

### Opmerkingen

**Kom meer te weten:**

* [Haal gegevens uit databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u gegevens uit de Sqlite-database kunt extraheren:

```csharp
// Maak een DbConnection-object
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Maak een instantie van de klasse Parser om tabellen uit de database te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleer of tekstextractie wordt ondersteund
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Controleer of toc-extractie wordt ondersteund
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Krijg een lijst met tabellen
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itereren over tabellen
    foreach (TocItem i in toc)
    {
        // Druk de tabelnaam af
        Console.WriteLine(i.Text);
        // Extraheer een tabelinhoud als tekst
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klasse om gegevens uit een database te extraheren.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connection | DbConnection | De databaseverbinding. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Kom meer te weten:**

* [Haal gegevens uit databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Loggen](https://docs.groupdocs.com/display/parsernet/Logging)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u gegevens uit de Sqlite-database kunt extraheren:

```csharp
// Maak een DbConnection-object
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Maak een instantie van de klasse Parser om tabellen uit de database te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleer of tekstextractie wordt ondersteund
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Controleer of toc-extractie wordt ondersteund
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Krijg een lijst met tabellen
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itereren over tabellen
    foreach (TocItem i in toc)
    {
        // Druk de tabelnaam af
        Console.WriteLine(i.Text);
        // Extraheer een tabelinhoud als tekst
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
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) class om gegevens te extraheren van een externe e-mailserver.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connection | EmailConnection | De e-mailverbinding. |

### Opmerkingen

**Kom meer te weten:**

* [Extraheer e-mails van een externe server via POP-, IMAP- of Exchange Web Services-protocollen](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u e-mails van Exchange Server kunt extraheren:

```csharp
// Maak het verbindingsobject voor het Exchange Web Services-protocol 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Maak een instantie van de Parser-klasse om e-mails van de externe server te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleer of containerextractie wordt ondersteund
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
        // Maak een exemplaar van de Parser-klasse voor e-mailberichten
        using (Parser emailParser = item.OpenParser())
        {
            // Extraheer de e-mailtekst
            using (TextReader reader = emailParser.GetText())
            {
                // Druk de e-mailtekst af
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Zie ook

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) class om gegevens te extraheren van een externe e-mailserver.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connection | EmailConnection | De e-mailverbinding. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Kom meer te weten:**

* [Extraheer e-mails van een externe server via POP-, IMAP- of Exchange Web Services-protocollen](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Loggen](https://docs.groupdocs.com/display/parsernet/Logging)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u e-mails van Exchange Server kunt extraheren:

```csharp
// Maak het verbindingsobject voor het Exchange Web Services-protocol 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Maak een instantie van de Parser-klasse om e-mails van de externe server te extraheren
using (Parser parser = new Parser(connection))
{
    // Controleer of containerextractie wordt ondersteund
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
        // Maak een exemplaar van de Parser-klasse voor e-mailberichten
        using (Parser emailParser = item.OpenParser())
        {
            // Extraheer de e-mailtekst
            using (TextReader reader = emailParser.GetText())
            {
                // Druk de e-mailtekst af
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
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klasse.

```csharp
public Parser(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |

### Opmerkingen

**Kom meer te weten:**

* [Laad document van lokale schijf](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u het document laadt vanaf de lokale schijf:

```csharp
// Maak een instantie van de Parser-klasse met het bestandspad
using (Parser parser = new Parser(filePath))
{
    // Extraheer een tekst in de reader
    using (TextReader reader = parser.GetText())
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een lezer null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klas mee[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |

### Opmerkingen

**Kom meer te weten:**

* [Specifieke bestandsindelingen laden](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Met een wachtwoord beveiligde documenten laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Laad document van lokale schijf](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Voorbeelden

Het documentwachtwoord wordt doorgegeven door de klasse LoadOptions:

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
        // Druk de documenttekst af
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Druk het bericht af als het wachtwoord onjuist of leeg is
    Console.WriteLine("Invalid password");
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klas mee[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

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
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klas mee[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) en[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het pad naar het bestand. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Kom meer te weten:**

* [Specifieke bestandsindelingen laden](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Met een wachtwoord beveiligde documenten laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Loggen](https://docs.groupdocs.com/display/parsernet/Logging)
* [Laad document van lokale schijf](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u de informatie kunt ontvangen via[`ILogger`](../../../groupdocs.parser.options/ilogger) koppel:

```csharp
// poging
{
    // Maak een instantie van de klasse Logger
    Logger logger = new Logger();
    // Maak een instantie van de Parser-klasse met de parser-instellingen
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Controleer of tekstextractie wordt ondersteund
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Druk de documenttekst af
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Negeer de uitzondering
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Foutmelding afdrukken
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Gebeurtenisbericht afdrukken
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Druk een waarschuwingsbericht af
        Console.WriteLine("Warning: " + message);
    }
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klasse.

```csharp
public Parser(Stream document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |

### Opmerkingen

**Kom meer te weten:**

* [Laad document uit stroom](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Voorbeelden

Het volgende voorbeeld laat zien hoe het document uit de stream moet worden geladen:

```csharp
// Maak een instantie van de Parser-klasse met de stream
using (Parser parser = new Parser(stream))
{
    // Extraheer een tekst in de reader
    using (TextReader reader = parser.GetText())
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een lezer null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klas mee[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |

### Opmerkingen

**Kom meer te weten:**

* [Specifieke bestandsindelingen laden](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Met een wachtwoord beveiligde documenten laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Laad document uit stroom](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Voorbeelden

In sommige gevallen is het nodig om te definiëren[`FileFormat`](../../../groupdocs.parser.options/fileformat). Zowel voor speciale gevallen (databases, e-mailserver) als voor het detecteren van bestandstypen door de inhoud:

Het documentwachtwoord wordt doorgegeven[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) klas:

```csharp
// Maak een exemplaar van de Parser-klasse voor een markdown-document
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
        // Druk de documenttekst af
        // Markdown is gedetecteerd; tekst zonder speciale symbolen wordt afgedrukt
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

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
        // Druk de documenttekst af
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Druk het bericht af als het wachtwoord onjuist of leeg is
    Console.WriteLine("Invalid password");
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klas mee[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

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
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initialiseert een nieuw exemplaar van het[`Parser`](../../parser) klas mee[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) en[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De broninvoerstroom. |
| loadOptions | LoadOptions | De opties om het bestand te openen. |
| parserSettings | ParserSettings | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |

### Opmerkingen

**Kom meer te weten:**

* [Specifieke bestandsindelingen laden](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Met een wachtwoord beveiligde documenten laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Laad document uit stroom](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Loggen](https://docs.groupdocs.com/display/parsernet/Logging)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u de informatie kunt ontvangen via[`ILogger`](../../../groupdocs.parser.options/ilogger) koppel:

```csharp
// poging
{
    // Maak een instantie van de klasse Logger
    Logger logger = new Logger();
    // Maak een instantie van de Parser-klasse met de parser-instellingen
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Controleer of tekstextractie wordt ondersteund
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Druk de documenttekst af
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Negeer de uitzondering
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Foutmelding afdrukken
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Gebeurtenisbericht afdrukken
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Druk een waarschuwingsbericht af
        Console.WriteLine("Warning: " + message);
    }
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
