---
title: "GetText"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Estrae un testo dal documento."
type: docs
weight: 180
url: /it/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Estrae un testo dal documento.

```csharp
public TextReader GetText()
```

### Valore di ritorno

Un'istanza della classe TextReader con il testo estratto; `null` se l'estrazione del testo non è supportata.

### Osservazioni

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Esempi

Il seguente esempio mostra come estrarre un testo da un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Estrai un testo nel lettore
    using(TextReader reader = parser.GetText())
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, il lettore è null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Vedi anche

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Estrae una pagina di testo dal documento usando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| options | TextOptions | Le opzioni di estrazione del testo. |

### Valore di ritorno

Un'istanza della classe TextReader con il testo estratto; `null` se l'estrazione del testo non è supportata.

### Osservazioni

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Esempi

Il seguente esempio mostra come estrarre un testo grezzo da un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Estrai un testo grezzo nel lettore
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, il lettore è null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Vedi anche

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Estrae un testo dalla pagina del documento.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |

### Valore di ritorno

Un'istanza della classe TextReader con il testo estratto; `null` se l'estrazione del testo della pagina non è supportata.

### Osservazioni

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Esempi

Il seguente esempio mostra come estrarre un testo dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione del testo
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Ottieni le informazioni del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Verifica se il documento ha pagine
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itera sulle pagine
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Estrai un testo nel lettore
        using(TextReader reader = parser.GetText(p))
        {
            // Stampa un testo dal documento
            // Ignoriamo il controllo di null poiché abbiamo già verificato il supporto della funzionalità di estrazione del testo.
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Vedi anche

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Estrae un testo dalla pagina del documento usando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |
| options | TextOptions | Le opzioni di estrazione del testo. |

### Valore di ritorno

Un'istanza della classe TextReader con il testo estratto; `null` se l'estrazione del testo della pagina non è supportata.

### Osservazioni

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Esempi

Il seguente esempio mostra come estrarre un testo grezzo dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione del testo
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Ottieni le informazioni del documento
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Verifica se il documento ha pagine
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itera sulle pagine
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Estrai un testo nel lettore
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Stampa un testo dal documento
            // Ignoriamo il controllo di null poiché abbiamo già verificato il supporto della funzionalità di estrazione del testo.
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Vedi anche

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
