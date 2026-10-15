---
title: "Parser"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Klasse Parsergroupdocs.parser/parser, um Daten von einer URI zu extrahieren."
type: docs
weight: 10
url: /de/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten von einer URI zu extrahieren.

```csharp
public Parser(Uri uri)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uri | Uri | Die URI, an die die Anforderung gesendet wird. |

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten von einer URI mit *loadOptions* zu extrahieren.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uri | Uri | Die URI, an die die Anforderung gesendet wird. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten von einer URI mit *parserSettings* zu extrahieren.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uri | Uri | Die URI, an die die Anforderung gesendet wird. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Siehe auch

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten von einer URI mit *loadOptions* und *parserSettings* zu extrahieren.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uri | Uri | Die URI, an die die Anforderung gesendet wird. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten aus einer Datenbank zu extrahieren.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verbindung | DbConnection | Die Datenbankverbindung. |

### Hinweise

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Beispiele

Das folgende Beispiel zeigt, wie man Daten aus einer Sqlite-Datenbank extrahiert:

```csharp
// Erstelle DbConnection-Objekt
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Erstelle eine Instanz der Parser-Klasse, um Tabellen aus der Datenbank zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen Sie, ob die Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Prüfen, ob die Extraktion des Inhaltsverzeichnisses unterstützt wird
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Erhalte eine Liste von Tabellen
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iteriere über Tabellen
    foreach (TocItem i in toc)
    {
        // Gib den Tabellennamen aus
        Console.WriteLine(i.Text);
        // Extrahiere den Tabelleninhalt als Text
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten aus einer Datenbank zu extrahieren.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verbindung | DbConnection | Die Datenbankverbindung. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Hinweise

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Beispiele

Das folgende Beispiel zeigt, wie man Daten aus einer Sqlite-Datenbank extrahiert:

```csharp
// Erstelle DbConnection-Objekt
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Erstelle eine Instanz der Parser-Klasse, um Tabellen aus der Datenbank zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen Sie, ob die Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Prüfen, ob die Extraktion des Inhaltsverzeichnisses unterstützt wird
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Erhalte eine Liste von Tabellen
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iteriere über Tabellen
    foreach (TocItem i in toc)
    {
        // Gib den Tabellennamen aus
        Console.WriteLine(i.Text);
        // Extrahiere den Tabelleninhalt als Text
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten von einem entfernten E-Mail-Server zu extrahieren.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verbindung | EmailConnection | Die E-Mail-Verbindung. |

### Hinweise

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Beispiele

Das folgende Beispiel zeigt, wie man E-Mails vom Exchange-Server extrahiert:

```csharp
// Erstelle das Verbindungsobjekt für das Exchange Web Services-Protokoll
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Erstelle eine Instanz der Parser-Klasse, um E-Mails vom entfernten Server zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen, ob die Container‑Extraktion unterstützt wird
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extrahiere E-Mail-Nachrichten vom Server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Durch Anhänge iterieren
    foreach (ContainerItem item in emails)
    {
        // Erstelle eine Instanz der Parser-Klasse für E-Mail-Nachrichten
        using (Parser emailParser = item.OpenParser())
        {
            // Extrahiere den E-Mail-Text
            using (TextReader reader = emailParser.GetText())
            {
                // Gib den E-Mail-Text aus
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Siehe auch

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse, um Daten von einem entfernten E-Mail-Server zu extrahieren.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verbindung | EmailConnection | Die E-Mail-Verbindung. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Hinweise

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Beispiele

Das folgende Beispiel zeigt, wie man E-Mails vom Exchange-Server extrahiert:

```csharp
// Erstelle das Verbindungsobjekt für das Exchange Web Services-Protokoll
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Erstelle eine Instanz der Parser-Klasse, um E-Mails vom entfernten Server zu extrahieren
using (Parser parser = new Parser(connection))
{
    // Prüfen, ob die Container‑Extraktion unterstützt wird
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extrahiere E-Mail-Nachrichten vom Server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Durch Anhänge iterieren
    foreach (ContainerItem item in emails)
    {
        // Erstelle eine Instanz der Parser-Klasse für E-Mail-Nachrichten
        using (Parser emailParser = item.OpenParser())
        {
            // Extrahiere den E-Mail-Text
            using (TextReader reader = emailParser.GetText())
            {
                // Gib den E-Mail-Text aus
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse.

```csharp
public Parser(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |

### Hinweise

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Beispiele

Das folgende Beispiel zeigt, wie man das Dokument von der lokalen Festplatte lädt:

```csharp
// Erstelle eine Instanz der Parser-Klasse mit dem Dateipfad
using (Parser parser = new Parser(filePath))
{
    // Text in den Reader extrahieren
    using (TextReader reader = parser.GetText())
    {
        // Text aus dem Dokument ausgeben
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse mit [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Hinweise

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Beispiele

Das Dokumentenpasswort wird von der LoadOptions-Klasse übergeben:

```csharp
try
{
    // Erstellen Sie eine Instanz der Parser-Klasse mit dem Passwort:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Prüfen Sie, ob die Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Geben Sie den Dokumenttext aus
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Geben Sie die Meldung aus, wenn das Passwort falsch oder leer ist
    Console.WriteLine("Invalid password");
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse mit [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Siehe auch

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse mit [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) und [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Hinweise

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Beispiele

Das folgende Beispiel zeigt, wie man die Informationen über die [`ILogger`](../../../groupdocs.parser.options/ilogger)-Schnittstelle erhält:

```csharp
// try
{
    // Erstellen Sie eine Instanz der Logger-Klasse
    Logger logger = new Logger();
    // Erstellen Sie eine Instanz der Parser-Klasse mit den Parser-Einstellungen
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Prüfen Sie, ob die Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Geben Sie den Dokumenttext aus
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
        // Geben Sie die Fehlermeldung aus
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Geben Sie die Ereignismeldung aus
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Geben Sie die Warnmeldung aus
        Console.WriteLine("Warning: " + message);
    }
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse.

```csharp
public Parser(Stream document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Der Quell-Eingabestream. |

### Hinweise

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Beispiele

Das folgende Beispiel zeigt, wie das Dokument aus dem Stream geladen wird:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse mit dem Stream
using (Parser parser = new Parser(stream))
{
    // Text in den Reader extrahieren
    using (TextReader reader = parser.GetText())
    {
        // Text aus dem Dokument ausgeben
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse mit [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Der Quell-Eingabestream. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Hinweise

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Beispiele

In manchen Fällen ist es notwendig, [`FileFormat`](../../../groupdocs.parser.options/fileformat) zu definieren. Sowohl für Sonderfälle (Datenbanken, E-Mail-Server) als auch zur Erkennung von Dateitypen anhand des Inhalts:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse für ein Markdown-Dokument
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Prüfen Sie, ob die Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Geben Sie den Dokumenttext aus
        // Markdown wird erkannt; Text ohne Sonderzeichen wird ausgegeben
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

Das Dokumentenpasswort wird über die [`LoadOptions`](../../../groupdocs.parser.options/loadoptions)-Klasse übergeben:

```csharp
try
{
    // Erstellen Sie eine Instanz der Parser-Klasse mit dem Passwort:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Prüfen Sie, ob die Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Geben Sie den Dokumenttext aus
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Geben Sie die Meldung aus, wenn das Passwort falsch oder leer ist
    Console.WriteLine("Invalid password");
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse mit [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Der Quell-Eingabestream. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Siehe auch

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initialisiert eine neue Instanz der [`Parser`](../../parser)-Klasse mit [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) und [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Der Quell-Eingabestream. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |
| parserSettings | ParserSettings | Die Parsereinstellungen, die zum Anpassen der Datenerfassung verwendet werden. |

### Hinweise

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Beispiele

Das folgende Beispiel zeigt, wie man die Informationen über die [`ILogger`](../../../groupdocs.parser.options/ilogger)-Schnittstelle erhält:

```csharp
// try
{
    // Erstellen Sie eine Instanz der Logger-Klasse
    Logger logger = new Logger();
    // Erstellen Sie eine Instanz der Parser-Klasse mit den Parser-Einstellungen
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Prüfen Sie, ob die Textextraktion unterstützt wird
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Geben Sie den Dokumenttext aus
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
        // Geben Sie die Fehlermeldung aus
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Geben Sie die Ereignismeldung aus
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Geben Sie die Warnmeldung aus
        Console.WriteLine("Warning: " + message);
    }
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
