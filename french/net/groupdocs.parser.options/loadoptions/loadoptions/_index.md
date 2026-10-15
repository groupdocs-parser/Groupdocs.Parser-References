---
title: "LoadOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe LoadOptionsgroupdocs.parser.options/loadoptions avec un Passwordgroupdocs.parser.options/loadoptions/password vide, un FileFormatgroupdocs.parser.options/loadoptions/fileformat égal à Unknown et les encodages par défaut."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec un [`Password`](../password) vide, un [`FileFormat`](../fileformat) égal à Unknown et les encodages par défaut.

```csharp
public LoadOptions()
```

### Voir aussi

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| timeout | TimeSpan | Le TimeSpan qui représente le nombre de millisecondes à attendre. |

### Voir aussi

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec un [`FileFormat`](../fileformat) égal à Unknown et les encodages par défaut.

```csharp
public LoadOptions(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |

### Voir aussi

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec un [`Password`](../password) vide et les encodages par défaut.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |

### Voir aussi

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec le mot de passe et les encodages par défaut.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |

### Voir aussi

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec des encodages personnalisés.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
| encoding | Encoding | L'encodage du document. |
| defaultAnsiEncoding | Encoding | L'encodage ANSI par défaut qui est utilisé pour la détection d'encodage. |

### Voir aussi

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) entièrement personnalisée.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
| encoding | Encoding | L'encodage du document. |
| defaultAnsiEncoding | Encoding | L'encodage ANSI par défaut qui est utilisé pour la détection d'encodage. |
| timeout | TimeSpan | Le TimeSpan qui représente le nombre de millisecondes à attendre. |

### Voir aussi

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec un [`Password`](../password) vide et les encodages par défaut.

```csharp
public LoadOptions(FileType fileType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileType | FileType | Le type du fichier. |

### Voir aussi

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec le mot de passe et les encodages par défaut.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileType | FileType | Le type du fichier. |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |

### Voir aussi

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) avec des encodages personnalisés.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileType | FileType | Le type du fichier. |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
| encoding | Encoding | L'encodage du document. |
| defaultAnsiEncoding | Encoding | L'encodage ANSI par défaut qui est utilisé pour la détection d'encodage. |

### Voir aussi

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Initialise une nouvelle instance de la classe [`LoadOptions`](../../loadoptions) entièrement personnalisée.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileType | FileType | Le type du fichier. |
| password | Chaîne | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
| encoding | Encoding | L'encodage du document. |
| defaultAnsiEncoding | Encoding | L'encodage ANSI par défaut qui est utilisé pour la détection d'encodage. |
| timeout | TimeSpan | Le TimeSpan qui représente le nombre de millisecondes à attendre. |

### Voir aussi

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
