---
title: "GetFileInfo"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Renvoie les informations générales sur un fichier."
type: docs
weight: 260
url: /fr/net/groupdocs.parser/parser/getfileinfo/
---

## GetFileInfo(string) {#getfileinfo_2}

Renvoie les informations générales sur un fichier.

```csharp
public static FileInfo GetFileInfo(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |

### Valeur de retour

Une instance de la classe [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Exemples

Le code suivant montre comment vérifier si un fichier est protégé par mot de passe :

```csharp
// Obtenir les informations du fichier
Options.FileInfo info = Parser.GetFileInfo(filePath);
// Vérifier la propriété IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### Voir aussi

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(string, LoadOptions) {#getfileinfo_3}

Renvoie les informations générales sur un fichier.

```csharp
public static FileInfo GetFileInfo(string filePath, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Le chemin du fichier. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Valeur de retour

Une instance de la classe [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Exemples

Le code suivant montre comment vérifier le type de fichier du document protégé par mot de passe :

```csharp
// Obtenir les informations du fichier
Options.FileInfo info = Parser.GetFileInfo(filePath, new LoadOptions("password"));
// Vérifier la propriété IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Afficher le type de fichier
Console.WriteLine(info.FileType.ToString());
```

### Voir aussi

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream) {#getfileinfo}

Renvoie les informations générales sur un fichier.

```csharp
public static FileInfo GetFileInfo(Stream document)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |

### Valeur de retour

Une instance de la classe [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Exemples

Le code suivant montre comment vérifier si un fichier est protégé par mot de passe :

```csharp
// Obtenir les informations du fichier
Options.FileInfo info = Parser.GetFileInfo(document);
// Vérifier la propriété IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### Voir aussi

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream, LoadOptions) {#getfileinfo_1}

Renvoie les informations générales sur un fichier.

```csharp
public static FileInfo GetFileInfo(Stream document, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux d'entrée source. |
| loadOptions | LoadOptions | Les options pour ouvrir le fichier. |

### Valeur de retour

Une instance de la classe [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Exemples

Le code suivant montre comment vérifier le type de fichier du document protégé par mot de passe :

```csharp
// Obtenir les informations du fichier
Options.FileInfo info = Parser.GetFileInfo(document);
// Vérifier la propriété IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Afficher le type de fichier
Console.WriteLine(info.FileType.ToString());
```

### Voir aussi

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
