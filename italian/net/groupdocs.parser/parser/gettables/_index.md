---
title: "GetTables"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Estrae le tabelle dal documento."
type: docs
weight: 170
url: /it/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Estrae le tabelle dal documento.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| options | PageTableAreaOptions | Le opzioni per l'estrazione delle tabelle. |

### Valore di ritorno

Una collezione di oggetti [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` se l'estrazione delle tabelle non è supportata.

### Esempi

Il seguente esempio mostra come estrarre le tabelle dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione delle tabelle
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Crea il layout delle tabelle
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Crea le opzioni per l'estrazione delle tabelle
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Estrai le tabelle dal documento
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Itera sulle tabelle
    foreach (PageTableArea t in tables)
    {
        // Itera sulle righe
        for (int row = 0; row < t.RowCount; row++)
        {
            // Itera sulle colonne
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Ottieni la cella della tabella
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Stampa il testo della cella della tabella
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Vedi anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Estrae tabelle dalla pagina del documento.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |
| options | PageTableAreaOptions | Le opzioni per l'estrazione delle tabelle. |

### Valore di ritorno

Una collezione di oggetti [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` se l'estrazione delle tabelle non è supportata.

### Esempi

Il seguente esempio mostra come estrarre le tabelle dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione delle tabelle
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Crea il layout delle tabelle
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Crea le opzioni per l'estrazione delle tabelle
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Ottieni le informazioni del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Verifica se il documento ha pagine
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Itera sulle pagine
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Estrai le tabelle dalla pagina del documento
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Itera sulle tabelle
        foreach (PageTableArea t in tables)
        {
            // Itera sulle righe
            for (int row = 0; row < t.RowCount; row++)
            {
                // Itera sulle colonne
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Ottieni la cella della tabella
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Stampa il testo della cella della tabella
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Vedi anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Estrae le tabelle dal documento.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Valore di ritorno

Una collezione di oggetti [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` se l'estrazione delle tabelle non è supportata.

### Esempi

Il seguente esempio mostra come estrarre le tabelle dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione delle tabelle
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Estrai le tabelle dal documento
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Itera sulle tabelle
    foreach (PageTableArea t in tables)
    {
        // Itera sulle righe
        for (int row = 0; row < t.RowCount; row++)
        {
            // Itera sulle colonne
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Ottieni la cella della tabella
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Stampa il testo della cella della tabella
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Vedi anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Estrae tabelle dalla pagina del documento.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |

### Valore di ritorno

Una collezione di oggetti [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` se l'estrazione delle tabelle non è supportata.

### Esempi

Il seguente esempio mostra come estrarre le tabelle dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione delle tabelle
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Ottieni le informazioni del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Verifica se il documento ha pagine
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Itera sulle pagine
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Estrai le tabelle dalla pagina del documento
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Itera sulle tabelle
        foreach (PageTableArea t in tables)
        {
            // Itera sulle righe
            for (int row = 0; row < t.RowCount; row++)
            {
                // Itera sulle colonne
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Ottieni la cella della tabella
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Stampa il testo della cella della tabella
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Vedi anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
