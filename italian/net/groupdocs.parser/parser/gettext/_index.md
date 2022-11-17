---
title: GetText
second_title: Riferimento API GroupDocs.Parser per .NET
description: Estrae un testo dal documento.
type: docs
weight: 150
url: /it/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Estrae un testo dal documento.

```csharp
public TextReader GetText()
```

### Valore di ritorno

Un'istanza diTextReader classe con il testo estratto; `nullo` se l'estrazione del testo non è supportata.

### Osservazioni

**Scopri di più:**

* [Estrai il testo dai documenti](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Estrai il testo in modalità Accurata](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Esempi

L'esempio seguente mostra come estrarre un testo da un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Estrai un testo nel lettore
    using(TextReader reader = parser.GetText())
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, un lettore è nullo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Guarda anche

* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Estrae una pagina di testo dal documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida del testo non elaborato).

```csharp
public TextReader GetText(TextOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | TextOptions | Le opzioni di estrazione del testo. |

### Valore di ritorno

Un'istanza diTextReader classe con il testo estratto; `nullo` se l'estrazione del testo non è supportata.

### Osservazioni

**Scopri di più:**

* [Estrai il testo in modalità Accurata](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Estrai il testo in modalità Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Esempi

L'esempio seguente mostra come estrarre un testo non elaborato da un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Estrai un testo non elaborato nel lettore
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Stampa un testo dal documento
        // Se l'estrazione del testo non è supportata, un lettore è nullo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Guarda anche

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Estrae un testo dalla pagina del documento.

```csharp
public TextReader GetText(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |

### Valore di ritorno

Un'istanza diTextReader classe con il testo estratto; `nullo` se l'estrazione della pagina di testo non è supportata.

### Osservazioni

**Scopri di più:**

* [Estrai il testo in modalità Accurata](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Esempi

L'esempio seguente mostra come estrarre un testo dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione del testo
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Ottieni le informazioni sul documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controlla se il documento ha pagine
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
            // Ignoriamo il controllo null poiché abbiamo verificato in precedenza il supporto della funzione di estrazione del testo
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Guarda anche

* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Estrae un testo dalla pagina del documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida del testo non elaborato).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |
| options | TextOptions | Le opzioni di estrazione del testo. |

### Valore di ritorno

Un'istanza diTextReader classe con il testo estratto; `nullo` se l'estrazione della pagina di testo non è supportata.

### Osservazioni

**Scopri di più:**

* [Estrai il testo in modalità Accurata](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Estrai il testo in modalità Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Esempi

L'esempio seguente mostra come estrarre un testo non elaborato dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione del testo
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Ottieni le informazioni sul documento
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Controlla se il documento ha pagine
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
            // Ignoriamo il controllo null poiché abbiamo verificato in precedenza il supporto della funzione di estrazione del testo
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Guarda anche

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
