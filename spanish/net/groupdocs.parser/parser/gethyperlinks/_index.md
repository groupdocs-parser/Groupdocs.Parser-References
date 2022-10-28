---
title: GetHyperlinks
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae hipervínculos del documento.
type: docs
weight: 100
url: /es/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Extrae hipervínculos del documento.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Valor_devuelto

Una colección de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objetos; `nulo` si la extracción de hipervínculos no es compatible.

### Ejemplos

El siguiente ejemplo muestra cómo extraer todos los hipervínculos de todo el documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de hipervínculos
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extraer hipervínculos del documento
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Iterar sobre hipervínculos
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Imprime el texto del hipervínculo
        Console.WriteLine(h.Text);
        // Imprimir la URL del hipervínculo
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Ver también

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extrae hipervínculos de la página del documento.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |

### Valor_devuelto

Una colección de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objetos; `nulo` si la extracción de hipervínculos no es compatible.

### Ejemplos

El siguiente ejemplo muestra cómo extraer hipervínculos de la página del documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de hipervínculos
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
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
        // Extraer hipervínculos de la página del documento
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Iterar sobre hipervínculos
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Imprime el texto del hipervínculo
            Console.WriteLine(h.Text);
            // Imprimir la URL del hipervínculo
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Ver también

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extrae los hipervínculos del documento usando las opciones de personalización (para establecer el área rectangular que contiene los hipervínculos).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | PageAreaOptions | Las opciones para la extracción de hipervínculos. |

### Valor_devuelto

Una colección de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objetos; `nulo` si la extracción de hipervínculos no es compatible.

### Ejemplos

El siguiente ejemplo muestra cómo extraer hipervínculos del área de la página del documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de hipervínculos
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Crear las opciones que se utilizan para la extracción de hipervínculos
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extraer hipervínculos del área de la página del documento
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Iterar sobre hipervínculos
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Imprime el texto del hipervínculo
        Console.WriteLine(h.Text);
        // Imprimir la URL del hipervínculo
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Ver también

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extrae hipervínculos de la página del documento usando las opciones de personalización (para establecer el área rectangular que contiene los hipervínculos).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |
| options | PageAreaOptions | Las opciones para la extracción de hipervínculos. |

### Valor_devuelto

Una colección de[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objetos; `nulo` si la extracción de hipervínculos no es compatible.

### Ejemplos

El siguiente ejemplo muestra cómo extraer hipervínculos del área de la página del documento usando opciones de personalización:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de hipervínculos
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Obtener la información del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Comprobar si el documento tiene páginas
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Crear las opciones que se utilizan para la extracción de hipervínculos
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Iterar sobre páginas
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Imprimir un número de página 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extraer hipervínculos del área de la página del documento
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Iterar sobre hipervínculos
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Imprime el texto del hipervínculo
            Console.WriteLine(h.Text);
            // Imprimir la URL del hipervínculo
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Ver también

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
