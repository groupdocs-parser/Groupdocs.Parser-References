---
title: Parser
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Initialise une nouvelle instance duParsergroupdocs.parser/parser classe pour extraire des données dune base de données.
type: docs
weight: 10
url: /fr/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Initialise une nouvelle instance du[`Parser`](../../parser) classe pour extraire des données d'une base de données.

```csharp
public Parser(DbConnection connection)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| connection | DbConnection | La connexion à la base de données. |

### Remarques

**Apprendre encore plus:**

* [Extraire des données de bases de données](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Exemples

L'exemple suivant montre comment extraire des données de la base de données Sqlite :

```csharp
// Créer un objet DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crée une instance de la classe Parser pour extraire les tables de la base de données
using (Parser parser = new Parser(connection))
{
    // Vérifie si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Vérifie si l'extraction de la table des matières est prise en charge
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Récupère une liste de tables
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itération sur les tables
    foreach (TocItem i in toc)
    {
        // Affiche le nom de la table
        Console.WriteLine(i.Text);
        // Extraire le contenu d'un tableau sous forme de texte
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir également

* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initialise une nouvelle instance du[`Parser`](../../parser) classe pour extraire des données d'une base de données.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| connection | DbConnection | La connexion à la base de données. |
| parserSettings | ParserSettings | Les paramètres de l'analyseur qui sont utilisés pour personnaliser l'extraction des données. |

### Remarques

**Apprendre encore plus:**

* [Extraire des données de bases de données](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Enregistrement](https://docs.groupdocs.com/display/parsernet/Logging)

### Exemples

L'exemple suivant montre comment extraire des données de la base de données Sqlite :

```csharp
// Créer un objet DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crée une instance de la classe Parser pour extraire les tables de la base de données
using (Parser parser = new Parser(connection))
{
    // Vérifie si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Vérifie si l'extraction de la table des matières est prise en charge
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Récupère une liste de tables
    IEnumerable<TocItem> toc = parser.GetToc();
    // Itération sur les tables
    foreach (TocItem i in toc)
    {
        // Affiche le nom de la table
        Console.WriteLine(i.Text);
        // Extraire le contenu d'un tableau sous forme de texte
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Voir également

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initialise une nouvelle instance du[`Parser`](../../parser) classe pour extraire les données d'un serveur de messagerie distant.

```csharp
public Parser(EmailConnection connection)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| connection | EmailConnection | La connexion e-mail. |

### Remarques

**Apprendre encore plus:**

* [Extraire les e-mails du serveur distant via les protocoles POP, IMAP ou Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Exemples

L'exemple suivant montre comment extraire des e-mails d'Exchange Server :

```csharp
// Créer l'objet de connexion pour le protocole Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crée une instance de la classe Parser pour extraire les emails du serveur distant
using (Parser parser = new Parser(connection))
{
    // Vérifie si l'extraction du conteneur est prise en charge
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraire les e-mails du serveur
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itérer sur les pièces jointes
    foreach (ContainerItem item in emails)
    {
        // Crée une instance de la classe Parser pour le message électronique
        using (Parser emailParser = item.OpenParser())
        {
            // Extraire le texte de l'email
            using (TextReader reader = emailParser.GetText())
            {
                // Imprimer le texte de l'e-mail
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Voir également

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initialise une nouvelle instance du[`Parser`](../../parser) classe pour extraire les données d'un serveur de messagerie distant.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| connection | EmailConnection | La connexion e-mail. |
| parserSettings | ParserSettings | Les paramètres de l'analyseur qui sont utilisés pour personnaliser l'extraction des données. |

### Remarques

**Apprendre encore plus:**

* [Extraire les e-mails du serveur distant via les protocoles POP, IMAP ou Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Enregistrement](https://docs.groupdocs.com/display/parsernet/Logging)

### Exemples

L'exemple suivant montre comment extraire des e-mails d'Exchange Server :

```csharp
// Créer l'objet de connexion pour le protocole Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crée une instance de la classe Parser pour extraire les emails du serveur distant
using (Parser parser = new Parser(connection))
{
    // Vérifie si l'extraction du conteneur est prise en charge
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraire les e-mails du serveur
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Itérer sur les pièces jointes
    foreach (ContainerItem item in emails)
    {
        // Crée une instance de la classe Parser pour le message électronique
        using (Parser emailParser = item.OpenParser())
        {
            // Extraire le texte de l'email
            using (TextReader reader = emailParser.GetText())
            {
                // Imprimer le texte de l'e-mail
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Voir également

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Initialise une nouvelle instance du[`Parser`](../../parser) classe.

```csharp
public Parser(string filePath)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin d'accès au fichier. |

### Remarques

**Apprendre encore plus:**

* [Charger le document à partir du disque local](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exemples

L'exemple suivant montre comment charger le document à partir du disque local :

```csharp
// Crée une instance de la classe Parser avec le filePath
using (Parser parser = new Parser(filePath))
{
    // Extraire un texte dans le lecteur
    using (TextReader reader = parser.GetText())
    {
        // Imprime un texte du document
        // Si l'extraction de texte n'est pas supportée, un lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir également

* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Initialise une nouvelle instance du[`Parser`](../../parser) classe avec[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin d'accès au fichier. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Remarques

**Apprendre encore plus:**

* [Chargement de formats de fichiers spécifiques](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Chargement de documents protégés par mot de passe](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Charger le document à partir du disque local](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exemples

Le mot de passe du document est passé par la classe LoadOptions :

```csharp
try
{
    // Crée une instance de la classe Parser avec le mot de passe :
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Vérifie si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprimer le texte du document
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Affiche le message si le mot de passe est incorrect ou vide
    Console.WriteLine("Invalid password");
}
```

### Voir également

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Initialise une nouvelle instance du[`Parser`](../../parser) classe avec[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin d'accès au fichier. |
| parserSettings | ParserSettings | Les paramètres de l'analyseur qui sont utilisés pour personnaliser l'extraction des données. |

### Voir également

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Initialise une nouvelle instance du[`Parser`](../../parser) classe avec[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) et[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin d'accès au fichier. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |
| parserSettings | ParserSettings | Les paramètres de l'analyseur qui sont utilisés pour personnaliser l'extraction des données. |

### Remarques

**Apprendre encore plus:**

* [Chargement de formats de fichiers spécifiques](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Chargement de documents protégés par mot de passe](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Enregistrement](https://docs.groupdocs.com/display/parsernet/Logging)
* [Charger le document à partir du disque local](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Exemples

L'exemple suivant montre comment recevoir les informations via[`ILogger`](../../../groupdocs.parser.options/ilogger) interface:

```csharp
// essayer
{
    // Crée une instance de la classe Logger
    Logger logger = new Logger();
    // Crée une instance de la classe Parser avec les paramètres de l'analyseur
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Vérifie si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprimer le texte du document
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignorer l'exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Affiche le message d'erreur
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Affiche le message d'événement
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Affiche le message d'avertissement
        Console.WriteLine("Warning: " + message);
    }
}
```

### Voir également

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initialise une nouvelle instance du[`Parser`](../../parser) classe.

```csharp
public Parser(Stream document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |

### Remarques

**Apprendre encore plus:**

* [Charger le document à partir du flux](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Exemples

L'exemple suivant montre comment charger le document à partir du flux :

```csharp
// Crée une instance de la classe Parser avec le flux
using (Parser parser = new Parser(stream))
{
    // Extraire un texte dans le lecteur
    using (TextReader reader = parser.GetText())
    {
        // Imprime un texte du document
        // Si l'extraction de texte n'est pas supportée, un lecteur est nul
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Voir également

* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initialise une nouvelle instance du[`Parser`](../../parser) classe avec[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Remarques

**Apprendre encore plus:**

* [Chargement de formats de fichiers spécifiques](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Chargement de documents protégés par mot de passe](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Charger le document à partir du flux](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Exemples

Dans certains cas, il est nécessaire de définir[`FileFormat`](../../../groupdocs.parser.options/fileformat). Tant pour les cas particuliers (bases de données, serveur de messagerie) que pour détecter les types de fichiers par le contenu :

Le mot de passe du document est transmis par[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) classe:

```csharp
// Crée une instance de la classe Parser pour le document Markdown
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Vérifie si l'extraction de texte est prise en charge
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Imprimer le texte du document
        // Markdown est détecté ; le texte sans symboles spéciaux est imprimé
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Crée une instance de la classe Parser avec le mot de passe :
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Vérifie si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprimer le texte du document
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Affiche le message si le mot de passe est incorrect ou vide
    Console.WriteLine("Invalid password");
}
```

### Voir également

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Initialise une nouvelle instance du[`Parser`](../../parser) classe avec[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| parserSettings | ParserSettings | Les paramètres de l'analyseur qui sont utilisés pour personnaliser l'extraction des données. |

### Voir également

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initialise une nouvelle instance du[`Parser`](../../parser) classe avec[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) et[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |
| parserSettings | ParserSettings | Les paramètres de l'analyseur qui sont utilisés pour personnaliser l'extraction des données. |

### Remarques

**Apprendre encore plus:**

* [Chargement de formats de fichiers spécifiques](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Chargement de documents protégés par mot de passe](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Charger le document à partir du flux](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Enregistrement](https://docs.groupdocs.com/display/parsernet/Logging)

### Exemples

L'exemple suivant montre comment recevoir les informations via[`ILogger`](../../../groupdocs.parser.options/ilogger) interface:

```csharp
// essayer
{
    // Crée une instance de la classe Logger
    Logger logger = new Logger();
    // Crée une instance de la classe Parser avec les paramètres de l'analyseur
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Vérifie si l'extraction de texte est prise en charge
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprimer le texte du document
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignorer l'exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Affiche le message d'erreur
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Affiche le message d'événement
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Affiche le message d'avertissement
        Console.WriteLine("Warning: " + message);
    }
}
```

### Voir également

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
