---
title: "LoadOptions"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Inizializza una nuova istanza della classe LoadOptionsgroupdocs.parser.options/loadoptions con Passwordgroupdocs.parser.options/loadoptions/password vuoto e FileFormatgroupdocs.parser.options/loadoptions/fileformat uguale a Unknown e codifiche predefinite."
type: docs
weight: 10
url: /it/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con [`Password`](../password) vuoto, [`FileFormat`](../fileformat) uguale a Unknown e codifiche predefinite.

```csharp
public LoadOptions()
```

### Vedi anche

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| timeout | TimeSpan | Il TimeSpan che rappresenta il numero di millisecondi da attendere. |

### Vedi anche

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con [`FileFormat`](../fileformat) uguale a Unknown e codifiche predefinite.

```csharp
public LoadOptions(string password)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| password | Stringa | La password per aprire il file protetto da password. |

### Vedi anche

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con [`Password`](../password) vuoto e codifiche predefinite.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileFormat | FileFormat | Il formato del file. |

### Vedi anche

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con la password e codifiche predefinite.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileFormat | FileFormat | Il formato del file. |
| password | Stringa | La password per aprire il file protetto da password. |

### Vedi anche

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con codifiche personalizzate.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileFormat | FileFormat | Il formato del file. |
| password | Stringa | La password per aprire il file protetto da password. |
| encoding | Encoding | La codifica del documento. |
| defaultAnsiEncoding | Encoding | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |

### Vedi anche

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) completamente personalizzata.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileFormat | FileFormat | Il formato del file. |
| password | Stringa | La password per aprire il file protetto da password. |
| encoding | Encoding | La codifica del documento. |
| defaultAnsiEncoding | Encoding | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
| timeout | TimeSpan | Il TimeSpan che rappresenta il numero di millisecondi da attendere. |

### Vedi anche

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con [`Password`](../password) vuoto e codifiche predefinite.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileType | FileType | Il tipo del file. |

### Vedi anche

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con la password e codifiche predefinite.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileType | FileType | Il tipo del file. |
| password | Stringa | La password per aprire il file protetto da password. |

### Vedi anche

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) con codifiche personalizzate.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileType | FileType | Il tipo del file. |
| password | Stringa | La password per aprire il file protetto da password. |
| encoding | Encoding | La codifica del documento. |
| defaultAnsiEncoding | Encoding | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |

### Vedi anche

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Inizializza una nuova istanza della classe [`LoadOptions`](../../loadoptions) completamente personalizzata.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| fileType | FileType | Il tipo del file. |
| password | Stringa | La password per aprire il file protetto da password. |
| encoding | Encoding | La codifica del documento. |
| defaultAnsiEncoding | Encoding | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
| timeout | TimeSpan | Il TimeSpan che rappresenta il numero di millisecondi da attendere. |

### Vedi anche

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
