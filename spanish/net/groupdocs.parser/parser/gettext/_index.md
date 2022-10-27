---
title: GetText
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae un texto del documento.
type: docs
weight: 150
url: /es/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Extrae un texto del documento.

```csharp
public TextReader GetText()
```

### Valor_devuelto

Una instancia deTextReader clase con el texto extraído; `nulo` si la extracción de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer texto de documentos](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extraer texto en modo Preciso](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Ejemplos

El siguiente ejemplo muestra cómo extraer un texto de un documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Extraer un texto en el lector
    using(TextReader reader = parser.GetText())
    {
        // Imprime un texto del documento
        // Si no se admite la extracción de texto, un lector es nulo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ver también

* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extrae una página de texto del documento usando las opciones de texto (para habilitar el modo de extracción rápida de texto sin formato).

```csharp
public TextReader GetText(TextOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | TextOptions | Las opciones de extracción de texto. |

### Valor_devuelto

Una instancia deTextReader clase con el texto extraído; `nulo` si la extracción de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer texto en modo Preciso](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraer texto en modo Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Ejemplos

El siguiente ejemplo muestra cómo extraer un texto sin procesar de un documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Extraer un texto sin procesar en el lector
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Imprime un texto del documento
        // Si no se admite la extracción de texto, un lector es nulo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ver también

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extrae un texto de la página del documento.

```csharp
public TextReader GetText(int pageIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |

### Valor_devuelto

Una instancia deTextReader clase con el texto extraído; `nulo` si la extracción de páginas de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer texto en modo Preciso](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Ejemplos

El siguiente ejemplo muestra cómo extraer un texto de la página del documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de texto
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Obtener la información del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Comprobar si el documento tiene páginas
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterar sobre páginas
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Imprimir un número de página 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extraer un texto en el lector
        using(TextReader reader = parser.GetText(p))
        {
            // Imprime un texto del documento
            // Ignoramos la verificación nula ya que hemos verificado la compatibilidad con la función de extracción de texto anteriormente
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ver también

* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extrae un texto de la página del documento usando las opciones de texto (para habilitar el modo de extracción rápida de texto sin formato).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |
| options | TextOptions | Las opciones de extracción de texto. |

### Valor_devuelto

Una instancia deTextReader clase con el texto extraído; `nulo` si la extracción de páginas de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer texto en modo Preciso](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraer texto en modo Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Ejemplos

El siguiente ejemplo muestra cómo extraer un texto sin formato de la página del documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de texto
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Obtener la información del documento
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Comprobar si el documento tiene páginas
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterar sobre páginas
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Imprimir un número de página 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extraer un texto en el lector
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Imprime un texto del documento
            // Ignoramos la verificación nula ya que hemos verificado la compatibilidad con la función de extracción de texto anteriormente
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ver también

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
