---
title: GetTables
second_title: Riferimento API GroupDocs.Parser per .NET
description: Estrae le tabelle dal documento.
type: docs
weight: 140
url: /it/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Estrae le tabelle dal documento.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | PageTableAreaOptions | Le opzioni per l'estrazione delle tabelle. |

### Valore di ritorno

Una raccolta di[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) oggetti; `nullo` se l'estrazione delle tabelle non è supportata.

### Esempi

L'esempio seguente mostra come estrarre le tabelle dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione della tabella
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Crea il layout delle tabelle
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Crea le opzioni per l'estrazione della tabella
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

### Guarda anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Estrae le tabelle dalla pagina del documento.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |
| options | PageTableAreaOptions | Le opzioni per l'estrazione delle tabelle. |

### Valore di ritorno

Una raccolta di[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) oggetti; `nullo` se l'estrazione delle tabelle non è supportata.

### Esempi

L'esempio seguente mostra come estrarre le tabelle dalla pagina del documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione della tabella
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Crea il layout delle tabelle
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Crea le opzioni per l'estrazione della tabella
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
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

### Guarda anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
