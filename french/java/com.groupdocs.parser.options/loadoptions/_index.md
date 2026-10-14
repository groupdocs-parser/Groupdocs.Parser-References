---
title: "LoadOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour ouvrir un fichier."
type: docs
weight: 24
url: /fr/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Fournit les options utilisées pour ouvrir un fichier.

Une instance de cette classe est utilisée comme paramètre dans les constructeurs de classe [Parser](../../com.groupdocs.parser/parser) :

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Voir les exemples d'utilisation là-bas.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec le délai d'attente. |
|
|  | [LoadOptions()](#LoadOptions--) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe vide, FileFormat égal à FileFormat.Unknown et les encodages par défaut. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec FileFormat égal à FileFormat.Unknown et les encodages par défaut. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe vide et les encodages par défaut. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec les encodages par défaut. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec des encodages personnalisés. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) entièrement personnalisée. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe vide et les encodages par défaut. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe et les encodages par défaut. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec des encodages personnalisés. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) entièrement personnalisée. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Obtient le format du fichier. |
|
|  | [getFileType()](#getFileType--) | Obtient le type de fichier. |
|
|  | [getPassword()](#getPassword--) | Obtient le mot de passe. |
|
|  | [getCharset()](#getCharset--) | Obtient l'encodage du document. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Obtient l'encodage ANSI par défaut utilisé pour la détection d'encodage. |
|
|  | [getTimeout()](#getTimeout--) | Obtient la valeur qui représente le nombre de millisecondes à attendre. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec le délai d'attente.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | timeout | java.time.Duration | La durée qui représente le nombre de millisecondes à attendre. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe vide, FileFormat égal à FileFormat.Unknown et les encodages par défaut.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec FileFormat égal à FileFormat.Unknown et les encodages par défaut.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe vide et les encodages par défaut.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Le format du fichier. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec les encodages par défaut.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Le format du fichier. |
|
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec des encodages personnalisés.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Le format du fichier. |
|
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|
|  | charset | java.nio.charset.Charset | L'encodage du document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | L'encodage ANSI par défaut utilisé pour la détection d'encodage. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) entièrement personnalisée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Le format du fichier. |
|
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|
|  | charset | java.nio.charset.Charset | L'encodage du document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | L'encodage ANSI par défaut utilisé pour la détection d'encodage. |
|
|  | timeout | java.time.Duration | La durée qui représente le nombre de millisecondes à attendre. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe vide et les encodages par défaut.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Le type du fichier. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec un mot de passe et les encodages par défaut.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Le type du fichier. |
|
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) avec des encodages personnalisés.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Le type du fichier. |
|
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|
|  | charset | java.nio.charset.Charset | L'encodage du document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | L'encodage ANSI par défaut utilisé pour la détection d'encodage. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) entièrement personnalisée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Le type du fichier. |
|
|  | password | java.lang.String | Le mot de passe pour ouvrir le fichier protégé par mot de passe. |
|
|  | charset | java.nio.charset.Charset | L'encodage du document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | L'encodage ANSI par défaut utilisé pour la détection d'encodage. |
|
|  | timeout | java.time.Duration | La durée qui représente le nombre de millisecondes à attendre. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Obtient le format du fichier.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Obtient le type de fichier.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Obtient le mot de passe.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le mot de passe pour ouvrir le fichier protégé par mot de passe.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Obtient l'encodage du document.


**Returns:**
java.nio.charset.Charset - Une instance de la classe Charset qui représente l'encodage du document ; null si elle n'est pas définie.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Obtient l'encodage ANSI par défaut utilisé pour la détection d'encodage.


**Returns:**
java.nio.charset.Charset - Une instance de la classe Charset qui représente l'encodage du document ; null si elle n'est pas définie.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Obtient la valeur qui représente le nombre de millisecondes à attendre.


**Returns:**
java.time.Duration - Une instance de Duration qui représente le nombre de millisecondes à attendre.

