---
title: "GetTextAreas"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Estrae aree di testo dal documento."
type: docs
weight: 190
url: /it/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

Estrae aree di testo dal documento.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Valore di ritorno

Una collezione di [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) oggetti; `null` se l'estrazione delle aree di testo non è supportata.

### Osservazioni

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Esempi

Il seguente esempio mostra come estrarre tutte le aree di testo dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Estrai le aree di testo
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Verifica se l'estrazione delle aree di testo è supportata
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itera sulle aree di testo della pagina
    foreach(PageTextArea a in areas)
    {
        // Stampa un indice di pagina, il rettangolo e il valore dell'area di testo:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Vedi anche

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Estrae aree di testo dal documento usando opzioni di personalizzazione (espressione regolare, distinzione maiuscole/minuscole, ecc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| options | PageTextAreaOptions | Le opzioni per l'estrazione delle aree di testo. |

### Valore di ritorno

Una collezione di [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) oggetti; `null` se l'estrazione delle aree di testo non è supportata.

### Osservazioni

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Esempi

Il seguente esempio mostra come estrarre solo le aree di testo con cifre dall'angolo in alto a sinistra:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Crea le opzioni utilizzate per l'estrazione delle aree di testo
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Estrai le aree di testo che contengono solo cifre dall'angolo in alto a sinistra di una pagina:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Verifica se l'estrazione delle aree di testo è supportata
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itera sulle aree di testo della pagina
    foreach(PageTextArea a in areas)
    {
        // Stampa un indice di pagina, il rettangolo e il valore dell'area di testo:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Vedi anche

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Estrae aree di testo dalla pagina del documento.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |

### Valore di ritorno

Una collezione di [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) oggetti; `null` se l'estrazione delle aree di testo non è supportata.

### Osservazioni

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Esempi

Per estrarre le aree di testo da una pagina di documento viene utilizzato il seguente metodo:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione delle aree di testo
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Ottieni le informazioni del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Verifica se il documento ha pagine
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itera sulle pagine
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Itera sulle aree di testo della pagina
        // Ignoriamo il controllo di null poiché abbiamo già verificato in precedenza il supporto della funzionalità di estrazione delle aree di testo
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Stampa un rettangolo e il valore dell'area di testo:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Vedi anche

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Estrae aree di testo dalla pagina del documento usando opzioni di personalizzazione (espressione regolare, distinzione maiuscole/minuscole, ecc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |
| options | PageTextAreaOptions | Le opzioni per l'estrazione delle aree di testo. |

### Valore di ritorno

Una collezione di [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) oggetti; `null` se l'estrazione delle aree di testo non è supportata.

### Osservazioni

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Vedi anche

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
