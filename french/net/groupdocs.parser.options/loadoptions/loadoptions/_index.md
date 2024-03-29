---
title: LoadOptions
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Initialise une nouvelle instance duLoadOptionsgroupdocs.parser.options/loadoptions classe avec videPasswordgroupdocs.parser.options/loadoptions/password FileFormatgroupdocs.parser.options/loadoptions/fileformat égal àUnknown et encodages par défaut.
type: docs
weight: 10
url: /fr/net/groupdocs.parser.options/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Initialise une nouvelle instance du[`LoadOptions`](../../loadoptions) classe avec vide[`Password`](../password) ,[`FileFormat`](../fileformat) égal àUnknown et encodages par défaut.

```csharp
public LoadOptions()
```

### Voir également

* class [LoadOptions](../../loadoptions)
* espace de noms [GroupDocs.Parser.Options](../../loadoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_4}

Initialise une nouvelle instance du[`LoadOptions`](../../loadoptions) classe avec[`FileFormat`](../fileformat) égal àUnknown et encodages par défaut.

```csharp
public LoadOptions(string password)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| password | String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |

### Voir également

* class [LoadOptions](../../loadoptions)
* espace de noms [GroupDocs.Parser.Options](../../loadoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Initialise une nouvelle instance du[`LoadOptions`](../../loadoptions) class avec vide[`Password`](../password)et encodages par défaut.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |

### Voir également

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* espace de noms [GroupDocs.Parser.Options](../../loadoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Initialise une nouvelle instance du[`LoadOptions`](../../loadoptions) classe avec le mot de passe et les encodages par défaut.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |
| password | String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |

### Voir également

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* espace de noms [GroupDocs.Parser.Options](../../loadoptions)
* Assemblée [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Initialise une nouvelle instance du[`LoadOptions`](../../loadoptions) classe avec des encodages personnalisés.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileFormat | FileFormat | Le format du fichier. |
| password | String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
| encoding | Encoding | L'encodage du document. |
| defaultAnsiEncoding | Encoding | Le codage ANSI par défaut utilisé pour la détection de codage. |

### Voir également

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* espace de noms [GroupDocs.Parser.Options](../../loadoptions)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
