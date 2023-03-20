---
title: GetTextAreas
second_title: GroupDocs.Parser voor .NET API-referentie
description: Extraheert tekstgebieden uit het document.
type: docs
weight: 160
url: /nl/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Extraheert tekstgebieden uit het document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Winstwaarde

Een verzameling van[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `nul` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekstgebieden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle tekstgebieden uit het hele document extraheert:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Extraheer tekstgebieden
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Controleer of extractie van tekstgebieden wordt ondersteund
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itereren over paginatekstgebieden
    foreach(PageTextArea a in areas)
    {
        // Druk een pagina-index, rechthoek en tekstgebiedwaarde af:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extraheert tekstgebieden uit het document met behulp van aanpassingsopties (reguliere expressie, hoofdletters, enz.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageTextAreaOptions | De opties voor extractie van tekstgebieden. |

### Winstwaarde

Een verzameling van[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `nul` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekstgebieden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alleen tekstgebieden met cijfers uit de linkerbovenhoek extraheert:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Maak de opties die worden gebruikt voor het extraheren van tekstgebieden
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extraheer tekstgebieden die alleen cijfers bevatten uit de linkerbovenhoek van een pagina:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Controleer of extractie van tekstgebieden wordt ondersteund
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itereren over paginatekstgebieden
    foreach(PageTextArea a in areas)
    {
        // Druk een pagina-index, rechthoek en tekstgebiedwaarde af:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extraheert tekstgebieden van de documentpagina.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |

### Winstwaarde

Een verzameling van[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `nul` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekstgebieden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voorbeelden

Om tekstgebieden uit een documentpagina te extraheren, wordt de volgende methode gebruikt:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Controleer of het document extractie van tekstgebieden ondersteunt
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Haal de documentinfo op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Herhaal pagina's
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Itereren over paginatekstgebieden
        // We negeren null-checking omdat we eerder de ondersteuning voor het extraheren van tekstgebieden hebben gecontroleerd
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Druk een rechthoek en tekstgebiedwaarde af:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extraheert tekstgebieden van de documentpagina met behulp van aanpassingsopties (reguliere expressie, hoofdletters, enz.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |
| options | PageTextAreaOptions | De opties voor extractie van tekstgebieden. |

### Winstwaarde

Een verzameling van[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `nul` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekstgebieden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
