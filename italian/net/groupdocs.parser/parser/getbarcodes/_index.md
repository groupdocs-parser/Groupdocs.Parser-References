---
title: "GetBarcodes"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Estrae i codici a barre dal documento."
type: docs
weight: 70
url: /it/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Estrae i codici a barre dal documento.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Valore di ritorno

Una collezione di oggetti [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` se l'estrazione dei codici a barre non è supportata.

### Esempi

Il seguente esempio mostra come estrarre i codici a barre da un documento:

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

### Vedi anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Estrae i codici a barre dalla pagina del documento.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |

### Valore di ritorno

Una collezione di oggetti [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` se l'estrazione dei codici a barre non è supportata.

### Esempi

Il seguente esempio mostra come estrarre i codici a barre da una pagina del documento:

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

### Vedi anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Estrae i codici a barre dal documento utilizzando le opzioni di personalizzazione.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| options | BarcodeOptions | Le opzioni per l'estrazione dei codici a barre. |

### Valore di ritorno

Una collezione di oggetti [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` se l'estrazione dei codici a barre non è supportata.

### Esempi

Il seguente esempio mostra come estrarre i codici a barre dall'angolo in alto a destra.

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Crea le opzioni utilizzate per l'estrazione dei codici a barre
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
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

### Vedi anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Estrae i codici a barre dalla pagina del documento utilizzando le opzioni di personalizzazione.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |
| options | BarcodeOptions | Le opzioni per l'estrazione dei codici a barre. |

### Valore di ritorno

Una collezione di oggetti [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` se l'estrazione dei codici a barre non è supportata.

### Vedi anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
