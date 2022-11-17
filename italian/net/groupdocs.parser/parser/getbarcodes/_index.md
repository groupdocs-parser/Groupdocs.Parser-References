---
title: GetBarcodes
second_title: Riferimento API GroupDocs.Parser per .NET
description: Estrae i codici a barre dal documento.
type: docs
weight: 50
url: /it/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Estrae i codici a barre dal documento.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Valore di ritorno

Una raccolta di[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) oggetti; `nullo` se l'estrazione dei codici a barre non è supportata.

### Esempi

L'esempio seguente mostra come estrarre i codici a barre da un documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Estrai i codici a barre dal documento.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Itera sui codici a barre
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Stampa l'indice della pagina
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Stampa il valore del codice a barre
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Guarda anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Estrae i codici a barre dalla pagina del documento.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |

### Valore di ritorno

Una raccolta di[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) oggetti; `nullo` se l'estrazione dei codici a barre non è supportata.

### Esempi

L'esempio seguente mostra come estrarre i codici a barre da una pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Estrai i codici a barre dalla seconda pagina del documento.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Itera sui codici a barre
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Stampa l'indice della pagina
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Stampa il valore del codice a barre
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Guarda anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Estrae i codici a barre dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | PageAreaOptions | Le opzioni per l'estrazione dei codici a barre. |

### Valore di ritorno

Una raccolta di[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) oggetti; `nullo` se l'estrazione dei codici a barre non è supportata.

### Esempi

L'esempio seguente mostra come estrarre i codici a barre dall'angolo in alto a destra.

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Crea le opzioni utilizzate per l'estrazione dei codici a barre
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Estrai i codici a barre dall'angolo in alto a destra.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Itera sui codici a barre
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Stampa l'indice della pagina
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Stampa il valore del codice a barre
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Guarda anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Estrae i codici a barre dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |
| options | PageAreaOptions | Le opzioni per l'estrazione dei codici a barre. |

### Valore di ritorno

Una raccolta di[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) oggetti; `nullo` se l'estrazione dei codici a barre non è supportata.

### Guarda anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
