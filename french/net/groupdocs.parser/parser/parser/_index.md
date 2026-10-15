---
title: "Analyseur"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe Parsergroupdocs.parser/parser pour extraire des données d'une URI."
type: docs
weight: 10
url: /fr/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'une URI.

```csharp
public Parser(Uri uri)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uri | Uri | L'URI vers lequel la requête est envoyée. |

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'une URI avec *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uri | Uri | L'URI vers lequel la requête est envoyée. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Voir aussi

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'une URI avec *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uri | Uri | L'URI vers lequel la requête est envoyée. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Voir aussi

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'une URI avec *loadOptions* et *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uri | Uri | L'URI vers lequel la requête est envoyée. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Voir aussi

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'une base de données.

```csharp
public Parser(DbConnection connection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connexion | DbConnection | La connexion à la base de données. |

### Remarques

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Exemples

L'exemple suivant montre comment extraire des données d'une base de données Sqlite :

```csharp
// Créer l'objet DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Créer une instance de la classe Parser pour extraire les tables de la base de données
using (Parser parser = new Parser(connection))
{
    // Vérifier si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Vérifier si l'extraction de la table des matières est prise en charge
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Obtenir la liste des tables
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itérer sur les tables
    foreach (TocItem i in toc)
    {
        // Afficher le nom de la table
        Console.WriteLine(i.Text);
        // Extraire le contenu d'une table sous forme de texte
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'une base de données.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connexion | DbConnection | La connexion à la base de données. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Remarques

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Exemples

L'exemple suivant montre comment extraire des données d'une base de données Sqlite :

```csharp
// Créer l'objet DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Créer une instance de la classe Parser pour extraire les tables de la base de données
using (Parser parser = new Parser(connection))
{
    // Vérifier si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Vérifier si l'extraction de la table des matières est prise en charge
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Obtenir la liste des tables
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itérer sur les tables
    foreach (TocItem i in toc)
    {
        // Afficher le nom de la table
        Console.WriteLine(i.Text);
        // Extraire le contenu d'une table sous forme de texte
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir aussi

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'un serveur de messagerie distant.

```csharp
public Parser(EmailConnection connection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connexion | EmailConnection | La connexion email. |

### Remarques

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Exemples

L'exemple suivant montre comment extraire des e‑mails depuis Exchange Server :

```csharp
// Créer l'objet de connexion pour le protocole Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Créer une instance de la classe Parser pour extraire les e‑mails du serveur distant
using (Parser parser = new Parser(connection))
{
    // Vérifier si l'extraction du conteneur est prise en charge
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraire les messages e‑mail du serveur
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Parcourir les pièces jointes
    foreach (ContainerItem item in emails)
    {
        // Créer une instance de la classe Parser pour le message courriel
        using (Parser emailParser = item.OpenParser())
        {
            // Extraire le texte du courriel
            using (TextReader reader = emailParser.GetText())
            {
                // Afficher le texte du courriel
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Voir aussi

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) pour extraire des données d'un serveur de messagerie distant.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connexion | EmailConnection | La connexion email. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Remarques

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Exemples

L'exemple suivant montre comment extraire des e‑mails depuis Exchange Server :

```csharp
// Créer l'objet de connexion pour le protocole Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Créer une instance de la classe Parser pour extraire les e‑mails du serveur distant
using (Parser parser = new Parser(connection))
{
    // Vérifier si l'extraction du conteneur est prise en charge
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraire les messages e‑mail du serveur
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Parcourir les pièces jointes
    foreach (ContainerItem item in emails)
    {
        // Créer une instance de la classe Parser pour le message courriel
        using (Parser emailParser = item.OpenParser())
        {
            // Extraire le texte du courriel
            using (TextReader reader = emailParser.GetText())
            {
                // Afficher le texte du courriel
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Voir aussi

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Initialise une nouvelle instance de la classe [`Parser`](../../parser).

```csharp
public Parser(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |

### Remarques

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exemples

L'exemple suivant montre comment charger le document depuis le disque local :

```csharp
// Créer une instance de la classe Parser avec le filePath
using (Parser parser = new Parser(filePath))
{
    // Extraire du texte dans le lecteur
    using (TextReader reader = parser.GetText())
    {
        // Afficher du texte depuis le document
        // Si l'extraction de texte n'est pas prise en charge, le lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) avec [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Remarques

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exemples

Le mot de passe du document est passé par la classe LoadOptions :

```csharp
try
{
    // Créer une instance de la classe Parser avec le mot de passe :
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Vérifier si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Afficher le texte du document
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Afficher le message si le mot de passe est incorrect ou vide
    Console.WriteLine("Invalid password");
}
```

### Voir aussi

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) avec [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Voir aussi

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) avec [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) et [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Remarques

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exemples

L'exemple suivant montre comment recevoir les informations via l'interface [`ILogger`](../../../groupdocs.parser.options/ilogger) :

```csharp
// try
{
    // Créer une instance de la classe Logger
    Logger logger = new Logger();
    // Créer une instance de la classe Parser avec les paramètres du parser
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Vérifier si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Afficher le texte du document
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
        // Afficher le message d'erreur
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Afficher le message d'événement
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Afficher le message d'avertissement
        Console.WriteLine("Warning: " + message);
    }
}
```

### Voir aussi

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initialise une nouvelle instance de la classe [`Parser`](../../parser).

```csharp
public Parser(Stream document)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |

### Remarques

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Exemples

L'exemple suivant montre comment charger le document depuis le flux :

```csharp
// Créer une instance de la classe Parser avec le flux
using (Parser parser = new Parser(stream))
{
    // Extraire du texte dans le lecteur
    using (TextReader reader = parser.GetText())
    {
        // Afficher du texte depuis le document
        // Si l'extraction de texte n'est pas prise en charge, le lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir aussi

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) avec [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Remarques

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Exemples

Dans certains cas, il est nécessaire de définir [`FileFormat`](../../../groupdocs.parser.options/fileformat). À la fois pour les cas spéciaux (bases de données, serveur de courriel) et pour détecter les types de fichiers à partir du contenu :

```csharp
// Créer une instance de la classe Parser pour le document markdown
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Vérifier si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Afficher le texte du document
        // Le markdown est détecté ; le texte sans symboles spéciaux est imprimé
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

Le mot de passe du document est transmis par la classe [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) :

```csharp
try
{
    // Créer une instance de la classe Parser avec le mot de passe :
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Vérifier si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Afficher le texte du document
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Afficher le message si le mot de passe est incorrect ou vide
    Console.WriteLine("Invalid password");
}
```

### Voir aussi

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) avec [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Voir aussi

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initialise une nouvelle instance de la classe [`Parser`](../../parser) avec [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) et [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |
| parserSettings | ParserSettings | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |

### Remarques

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Exemples

L'exemple suivant montre comment recevoir les informations via l'interface [`ILogger`](../../../groupdocs.parser.options/ilogger) :

```csharp
// try
{
    // Créer une instance de la classe Logger
    Logger logger = new Logger();
    // Créer une instance de la classe Parser avec les paramètres du parser
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Vérifier si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Afficher le texte du document
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
        // Afficher le message d'erreur
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Afficher le message d'événement
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Afficher le message d'avertissement
        Console.WriteLine("Warning: " + message);
    }
}
```

### Voir aussi

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
