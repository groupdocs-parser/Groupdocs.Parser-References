---
title: Parser
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Initialisiert eine neue Instanz vonParsergroupdocs.parser/parser Klasse zum Extrahieren von Daten aus einer Datenbank.
type: docs
weight: 10
url: /de/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse zum Extrahieren von Daten aus einer Datenbank.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connection | DbConnection | Die Datenbankverbindung. |

### Bemerkungen

**Mehr erfahren:**

* [Daten aus Datenbanken extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Beispiele

Das folgende Beispiel zeigt, wie Daten aus der Sqlite-Datenbank extrahiert werden:

```csharp
// DbConnection-Objekt erstellen
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Erstellen Sie eine Instanz der Parser-Klasse, um Tabellen aus der Datenbank zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen, ob Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Prüfen, ob toc-Extraktion unterstützt wird
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Holen Sie sich eine Liste von Tabellen
    IEnumerable<TocItem> toc = parser.GetToc();
    // Über Tabellen iterieren
    foreach (TocItem i in toc)
    {
        // Den Tabellennamen drucken
        Console.WriteLine(i.Text);
        // Tabelleninhalt als Text extrahieren
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse zum Extrahieren von Daten aus einer Datenbank.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connection | DbConnection | Die Datenbankverbindung. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenextraktion verwendet werden. |

### Bemerkungen

**Mehr erfahren:**

* [Daten aus Datenbanken extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Protokollierung](https://docs.groupdocs.com/display/parsernet/Logging)

### Beispiele

Das folgende Beispiel zeigt, wie Daten aus der Sqlite-Datenbank extrahiert werden:

```csharp
// DbConnection-Objekt erstellen
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Erstellen Sie eine Instanz der Parser-Klasse, um Tabellen aus der Datenbank zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen, ob Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Prüfen, ob toc-Extraktion unterstützt wird
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Holen Sie sich eine Liste von Tabellen
    IEnumerable<TocItem> toc = parser.GetToc();
    // Über Tabellen iterieren
    foreach (TocItem i in toc)
    {
        // Den Tabellennamen drucken
        Console.WriteLine(i.Text);
        // Tabelleninhalt als Text extrahieren
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse zum Extrahieren von Daten von einem Remote-E-Mail-Server.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connection | EmailConnection | Die E-Mail-Verbindung. |

### Bemerkungen

**Mehr erfahren:**

* [Extrahieren Sie E-Mails von Remote-Servern über POP-, IMAP- oder Exchange Web Services-Protokolle](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Beispiele

Das folgende Beispiel zeigt, wie Sie E-Mails von Exchange Server extrahieren:

```csharp
// Das Verbindungsobjekt für das Exchange Web Services-Protokoll erstellen 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Erstellen Sie eine Instanz der Parser-Klasse, um E-Mails vom Remote-Server zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen, ob die Container-Extraktion unterstützt wird
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// E-Mail-Nachrichten vom Server extrahieren
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Über Anhänge iterieren
    foreach (ContainerItem item in emails)
    {
        // Erstellen Sie eine Instanz der Parser-Klasse für die E-Mail-Nachricht
        using (Parser emailParser = item.OpenParser())
        {
            // E-Mail-Text extrahieren
            using (TextReader reader = emailParser.GetText())
            {
                // E-Mail-Text drucken
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Siehe auch

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse zum Extrahieren von Daten von einem Remote-E-Mail-Server.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connection | EmailConnection | Die E-Mail-Verbindung. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenextraktion verwendet werden. |

### Bemerkungen

**Mehr erfahren:**

* [Extrahieren Sie E-Mails von Remote-Servern über POP-, IMAP- oder Exchange Web Services-Protokolle](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Protokollierung](https://docs.groupdocs.com/display/parsernet/Logging)

### Beispiele

Das folgende Beispiel zeigt, wie Sie E-Mails von Exchange Server extrahieren:

```csharp
// Das Verbindungsobjekt für das Exchange Web Services-Protokoll erstellen 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Erstellen Sie eine Instanz der Parser-Klasse, um E-Mails vom Remote-Server zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen, ob die Container-Extraktion unterstützt wird
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// E-Mail-Nachrichten vom Server extrahieren
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Über Anhänge iterieren
    foreach (ContainerItem item in emails)
    {
        // Erstellen Sie eine Instanz der Parser-Klasse für die E-Mail-Nachricht
        using (Parser emailParser = item.OpenParser())
        {
            // E-Mail-Text extrahieren
            using (TextReader reader = emailParser.GetText())
            {
                // E-Mail-Text drucken
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Siehe auch

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_7}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse.

```csharp
public Parser(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |

### Bemerkungen

**Mehr erfahren:**

* [Dokument von lokaler Festplatte laden](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Beispiele

Das folgende Beispiel zeigt, wie das Dokument von der lokalen Festplatte geladen wird:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse mit dem Dateipfad
using (Parser parser = new Parser(filePath))
{
    // Einen Text in den Reader extrahieren
    using (TextReader reader = parser.GetText())
    {
        // Einen Text aus dem Dokument drucken
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_8}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse mit[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Bemerkungen

**Mehr erfahren:**

* [Laden bestimmter Dateiformate](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Passwortgeschützte Dokumente laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Dokument von lokaler Festplatte laden](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Beispiele

Das Dokumentpasswort wird von der LoadOptions-Klasse übergeben:

```csharp
try
{
    // Erstellen Sie eine Instanz der Parser-Klasse mit dem Passwort:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Prüfen, ob Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Dokumenttext drucken
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Gibt die Nachricht aus, wenn das Passwort falsch oder leer ist
    Console.WriteLine("Invalid password");
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_9}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse mit[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) und[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenextraktion verwendet werden. |

### Bemerkungen

**Mehr erfahren:**

* [Laden bestimmter Dateiformate](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Passwortgeschützte Dokumente laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Protokollierung](https://docs.groupdocs.com/display/parsernet/Logging)
* [Dokument von lokaler Festplatte laden](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Beispiele

Das folgende Beispiel zeigt, wie Sie die Informationen per erhalten[`ILogger`](../../../groupdocs.parser.options/ilogger) Schnittstelle:

```csharp
// Versuchen
{
    // Erstellen Sie eine Instanz der Logger-Klasse
    Logger logger = new Logger();
    // Eine Instanz der Parser-Klasse mit den Parser-Einstellungen erstellen
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Prüfen, ob Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Dokumenttext drucken
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ausnahme ignorieren
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Fehlermeldung drucken
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Ereignismeldung drucken
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Warnmeldung drucken
        Console.WriteLine("Warning: " + message);
    }
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse.

```csharp
public Parser(Stream document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | Stream | Der Quelleingabestream. |

### Bemerkungen

**Mehr erfahren:**

* [Dokument aus Stream laden](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Beispiele

Das folgende Beispiel zeigt, wie das Dokument aus dem Stream geladen wird:

```csharp
// Eine Instanz der Parser-Klasse mit dem Stream erstellen
using (Parser parser = new Parser(stream))
{
    // Einen Text in den Reader extrahieren
    using (TextReader reader = parser.GetText())
    {
        // Einen Text aus dem Dokument drucken
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse mit[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | Stream | Der Quelleingabestream. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Bemerkungen

**Mehr erfahren:**

* [Laden bestimmter Dateiformate](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Passwortgeschützte Dokumente laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Dokument aus Stream laden](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Beispiele

In einigen Fällen ist eine Definition erforderlich[`FileFormat`](../../../groupdocs.parser.options/fileformat). Sowohl für Sonderfälle (Datenbanken, E-Mail-Server) als auch zur Erkennung von Dateitypen anhand des Inhalts:

Das Dokumentenkennwort wird übergeben[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) Klasse:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse für das Markdown-Dokument
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Prüfen, ob Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Dokumenttext drucken
        // Markdown wird erkannt; Text ohne Sonderzeichen wird gedruckt
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Erstellen Sie eine Instanz der Parser-Klasse mit dem Passwort:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Prüfen, ob Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Dokumenttext drucken
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Gibt die Nachricht aus, wenn das Passwort falsch oder leer ist
    Console.WriteLine("Invalid password");
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initialisiert eine neue Instanz von[`Parser`](../../parser) Klasse mit[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) und[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | Stream | Der Quelleingabestream. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenextraktion verwendet werden. |

### Bemerkungen

**Mehr erfahren:**

* [Laden bestimmter Dateiformate](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Passwortgeschützte Dokumente laden](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Dokument aus Stream laden](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Protokollierung](https://docs.groupdocs.com/display/parsernet/Logging)

### Beispiele

Das folgende Beispiel zeigt, wie Sie die Informationen per erhalten[`ILogger`](../../../groupdocs.parser.options/ilogger) Schnittstelle:

```csharp
// Versuchen
{
    // Erstellen Sie eine Instanz der Logger-Klasse
    Logger logger = new Logger();
    // Eine Instanz der Parser-Klasse mit den Parser-Einstellungen erstellen
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Prüfen, ob Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Dokumenttext drucken
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ausnahme ignorieren
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Fehlermeldung drucken
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Ereignismeldung drucken
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Warnmeldung drucken
        Console.WriteLine("Warning: " + message);
    }
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
