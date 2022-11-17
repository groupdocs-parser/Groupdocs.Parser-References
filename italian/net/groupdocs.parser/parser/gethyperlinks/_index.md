---
title: GetHyperlinks
second_title: Riferimento API GroupDocs.Parser per .NET
description: Estrae i collegamenti ipertestuali dal documento.
type: docs
weight: 100
url: /it/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Estrae i collegamenti ipertestuali dal documento.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Valore di ritorno

Una raccolta di[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) oggetti; `nullo` se l'estrazione dei collegamenti ipertestuali non è supportata.

### Esempi

L'esempio seguente mostra come estrarre tutti i collegamenti ipertestuali dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione del collegamento ipertestuale
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Estrai i collegamenti ipertestuali dal documento
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Itera sui collegamenti ipertestuali
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Stampa il testo del collegamento ipertestuale
        Console.WriteLine(h.Text);
        // Stampa l'URL del collegamento ipertestuale
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Guarda anche

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Estrae i collegamenti ipertestuali dalla pagina del documento.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |

### Valore di ritorno

Una raccolta di[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) oggetti; `nullo` se l'estrazione dei collegamenti ipertestuali non è supportata.

### Esempi

L'esempio seguente mostra come estrarre i collegamenti ipertestuali dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione del collegamento ipertestuale
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Ottieni le informazioni sul documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controlla se il documento ha pagine
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Itera sulle pagine
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Estrai i collegamenti ipertestuali dalla pagina del documento
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Itera sui collegamenti ipertestuali
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Stampa il testo del collegamento ipertestuale
            Console.WriteLine(h.Text);
            // Stampa l'URL del collegamento ipertestuale
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Guarda anche

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Estrae i collegamenti ipertestuali dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | PageAreaOptions | Le opzioni per l'estrazione dei collegamenti ipertestuali. |

### Valore di ritorno

Una raccolta di[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) oggetti; `nullo` se l'estrazione dei collegamenti ipertestuali non è supportata.

### Esempi

L'esempio seguente mostra come estrarre i collegamenti ipertestuali dall'area della pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione del collegamento ipertestuale
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Crea le opzioni utilizzate per l'estrazione del collegamento ipertestuale
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Estrai i collegamenti ipertestuali dall'area della pagina del documento
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Itera sui collegamenti ipertestuali
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Stampa il testo del collegamento ipertestuale
        Console.WriteLine(h.Text);
        // Stampa l'URL del collegamento ipertestuale
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Guarda anche

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Estrae i collegamenti ipertestuali dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |
| options | PageAreaOptions | Le opzioni per l'estrazione dei collegamenti ipertestuali. |

### Valore di ritorno

Una raccolta di[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) oggetti; `nullo` se l'estrazione dei collegamenti ipertestuali non è supportata.

### Esempi

L'esempio seguente mostra come estrarre i collegamenti ipertestuali dall'area della pagina del documento utilizzando le opzioni di personalizzazione:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione del collegamento ipertestuale
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Ottieni le informazioni sul documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controlla se il documento ha pagine
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Crea le opzioni utilizzate per l'estrazione del collegamento ipertestuale
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Itera sulle pagine
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Estrai i collegamenti ipertestuali dall'area della pagina del documento
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Itera sui collegamenti ipertestuali
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Stampa il testo del collegamento ipertestuale
            Console.WriteLine(h.Text);
            // Stampa l'URL del collegamento ipertestuale
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Guarda anche

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
