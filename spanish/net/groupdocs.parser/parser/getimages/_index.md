---
title: GetImages
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae imágenes del documento.
type: docs
weight: 110
url: /es/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Extrae imágenes del documento.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Valor_devuelto

Una colección de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objetos; `nulo` si la extracción de imágenes no es compatible.

### Observaciones

**Aprende más:**

* [Extraer imágenes de documentos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraer imágenes a archivos](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraiga imágenes de documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraer imágenes de hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraiga imágenes de presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraer imágenes de correos electrónicos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraer imágenes de documentos PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Ejemplos

El siguiente ejemplo muestra cómo extraer todas las imágenes de todo el documento:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Extraer imágenes
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Comprobar si se admite la extracción de imágenes
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Iterar sobre imágenes
    foreach (PageImageArea image in images)
    {
        // Imprimir un índice de página, un rectángulo y un tipo de imagen:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Ver también

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Extrae imágenes del documento usando las opciones de personalización (para establecer el área rectangular que contiene las imágenes).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | PageAreaOptions | Las opciones para la extracción de imágenes. |

### Valor_devuelto

Una colección de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objetos; `nulo` si la extracción de imágenes no es compatible.

### Observaciones

**Aprende más:**

* [Extraer imágenes de documentos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraer imágenes a archivos](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraer imágenes del área de la página del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extraiga imágenes de documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraer imágenes de hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraiga imágenes de presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraer imágenes de correos electrónicos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraer imágenes de documentos PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Ejemplos

El siguiente ejemplo muestra cómo extraer solo imágenes de la esquina superior izquierda:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Crear las opciones que se utilizan para la extracción de imágenes.
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Extraer imágenes de la esquina superior izquierda de una página:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Comprobar si se admite la extracción de imágenes
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Iterar sobre imágenes
    foreach (PageImageArea image in images)
    {
        // Imprimir un índice de página, un rectángulo y un tipo de imagen:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Ver también

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Extrae imágenes de la página del documento.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |

### Valor_devuelto

Una colección de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objetos; `nulo` si la extracción de imágenes no es compatible.

### Observaciones

**Aprende más:**

* [Extraer imágenes de documentos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraer imágenes a archivos](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraer imágenes de la página del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extraiga imágenes de documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraer imágenes de hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraiga imágenes de presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraer imágenes de correos electrónicos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraer imágenes de documentos PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Ejemplos

Para extraer imágenes de una página de documento se utiliza el siguiente método:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de imágenes
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Imprimir un número de página 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Iterar sobre imágenes
        // Ignoramos la verificación nula ya que hemos verificado la compatibilidad con la función de extracción de imágenes anteriormente
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Imprime un rectángulo y un tipo de imagen
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Ver también

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Extrae imágenes de la página del documento usando las opciones de personalización (para establecer el área rectangular que contiene las imágenes).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |
| options | PageAreaOptions | Las opciones para la extracción de imágenes. |

### Valor_devuelto

Una colección de[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objetos; `nulo` si la extracción de imágenes no es compatible.

### Observaciones

**Aprende más:**

* [Extraer imágenes de documentos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraer imágenes a archivos](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraer imágenes de la página del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extraer imágenes del área de la página del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extraiga imágenes de documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraer imágenes de hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraiga imágenes de presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraer imágenes de correos electrónicos](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraer imágenes de documentos PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Ver también

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
