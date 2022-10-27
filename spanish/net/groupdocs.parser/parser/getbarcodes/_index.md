---
title: GetBarcodes
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae códigos de barras del documento.
type: docs
weight: 50
url: /es/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Extrae códigos de barras del documento.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Valor_devuelto

Una colección de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objetos; `nulo` si no se admite la extracción de códigos de barras.

### Ejemplos

El siguiente ejemplo muestra cómo extraer códigos de barras de un documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Extraer códigos de barras del documento.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Iterar sobre códigos de barras
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Imprime el índice de la página
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Imprime el valor del código de barras
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Ver también

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Extrae códigos de barras de la página del documento.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |

### Valor_devuelto

Una colección de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objetos; `nulo` si no se admite la extracción de códigos de barras.

### Ejemplos

El siguiente ejemplo muestra cómo extraer códigos de barras de una página de documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Extraer códigos de barras de la segunda página del documento.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Iterar sobre códigos de barras
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Imprime el índice de la página
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Imprime el valor del código de barras
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Ver también

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Extrae códigos de barras del documento usando las opciones de personalización (para configurar el área rectangular que contiene códigos de barras).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | PageAreaOptions | Las opciones para la extracción de códigos de barras. |

### Valor_devuelto

Una colección de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objetos; `nulo` si no se admite la extracción de códigos de barras.

### Ejemplos

El siguiente ejemplo muestra cómo extraer códigos de barras de la esquina superior derecha.

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Crear las opciones que se utilizan para la extracción de códigos de barras
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extrae los códigos de barras de la esquina superior derecha.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Iterar sobre códigos de barras
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Imprime el índice de la página
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Imprime el valor del código de barras
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Ver también

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Extrae códigos de barras de la página del documento usando las opciones de personalización (para establecer el área rectangular que contiene códigos de barras).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |
| options | PageAreaOptions | Las opciones para la extracción de códigos de barras. |

### Valor_devuelto

Una colección de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objetos; `nulo` si no se admite la extracción de códigos de barras.

### Ver también

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
