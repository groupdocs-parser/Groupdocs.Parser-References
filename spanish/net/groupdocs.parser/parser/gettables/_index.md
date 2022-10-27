---
title: GetTables
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae tablas del documento.
type: docs
weight: 140
url: /es/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Extrae tablas del documento.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | PageTableAreaOptions | Las opciones para la extracción de tablas. |

### Valor_devuelto

Una colección de[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objetos; `nulo` si la extracción de tablas no es compatible.

### Ejemplos

El siguiente ejemplo muestra cómo extraer tablas de todo el documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de tablas
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Crear el diseño de las tablas
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Crea las opciones para la extracción de tablas.
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extraer tablas del documento
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Iterar sobre tablas
    foreach (PageTableArea t in tables)
    {
        // Iterar sobre filas
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iterar sobre columnas
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Obtener la celda de la tabla
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Imprime el texto de la celda de la tabla
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

### Ver también

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Extrae tablas de la página del documento.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |
| options | PageTableAreaOptions | Las opciones para la extracción de tablas. |

### Valor_devuelto

Una colección de[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objetos; `nulo` si la extracción de tablas no es compatible.

### Ejemplos

El siguiente ejemplo muestra cómo extraer tablas de la página del documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de tablas
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Crear el diseño de las tablas
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Crea las opciones para la extracción de tablas.
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Obtener la información del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Comprobar si el documento tiene páginas
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iterar sobre páginas
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Imprimir un número de página 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraer tablas de la página del documento
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Iterar sobre tablas
        foreach (PageTableArea t in tables)
        {
            // Iterar sobre filas
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iterar sobre columnas
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Obtener la celda de la tabla
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Imprime el texto de la celda de la tabla
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

### Ver también

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
