---
title: "LoadOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options utilisées pour ouvrir un fichier."
type: docs
weight: 420
url: /fr/net/groupdocs.parser.options/loadoptions/
---

## LoadOptions class

Fournit les options utilisées pour ouvrir un fichier.

```csharp
public sealed class LoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec un [`Password`](./password) vide, [`FileFormat`](./fileformat) égal à Unknown et les encodages par défaut. |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec un [`Password`](./password) vide et les encodages par défaut. |
| [LoadOptions](loadoptions#constructor_5)(FileType) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec un [`Password`](./password) vide et les encodages par défaut. |
| [LoadOptions](loadoptions#constructor_9)(string) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec [`FileFormat`](./fileformat) égal à Unknown et les encodages par défaut. |
| [LoadOptions](loadoptions#constructor_10)(TimeSpan) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec *timeout*. |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec le mot de passe et les encodages par défaut. |
| [LoadOptions](loadoptions#constructor_6)(FileType, string) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec le mot de passe et les encodages par défaut. |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec des encodages personnalisés. |
| [LoadOptions](loadoptions#constructor_7)(FileType, string, Encoding, Encoding) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) avec des encodages personnalisés. |
| [LoadOptions](loadoptions#constructor_4)(FileFormat, string, Encoding, Encoding, TimeSpan) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) entièrement personnalisée. |
| [LoadOptions](loadoptions#constructor_8)(FileType, string, Encoding, Encoding, TimeSpan) | Initialise une nouvelle instance de la classe [`LoadOptions`](../loadoptions) entièrement personnalisée. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | Obtient l'encodage ANSI par défaut utilisé pour la détection d'encodage. |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | Obtient l'encodage du document. |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | Obtient le format du fichier. |
| [FileType](../../groupdocs.parser.options/loadoptions/filetype) { get; } | Obtient le type de fichier. |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | Obtient le mot de passe. |
| [Timeout](../../groupdocs.parser.options/loadoptions/timeout) { get; } | Obtient la valeur qui représente le nombre de millisecondes à attendre. |

### Remarques

Une instance de cette classe est utilisée comme paramètre dans les constructeurs de la classe [`Parser`](../../groupdocs.parser/parser) :

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

Voir les exemples d'utilisation là-bas.

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
