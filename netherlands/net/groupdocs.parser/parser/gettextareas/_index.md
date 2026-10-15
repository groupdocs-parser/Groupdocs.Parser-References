---
title: "GetTextAreas"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Extraheert tekstgebieden uit het document."
type: docs
weight: 190
url: /nl/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

Extraheert tekstgebieden uit het document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Retourwaarde

Een collectie van [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `null` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voorbeelden

Het volgende voorbeeld toont hoe alle tekstgebieden uit het volledige document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
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
 
    // Itereer over paginatekstgebieden
    foreach(PageTextArea a in areas)
    {
        // Print een pagina-index, rechthoek en tekstgebiedwaarde:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extraheert tekstgebieden uit het document met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoeligheid, enz.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageTextAreaOptions | De opties voor extractie van tekstgebieden. |

### Retourwaarde

Een collectie van [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `null` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voorbeelden

Het volgende voorbeeld toont hoe alleen tekstgebieden met cijfers uit de linkerbovenhoek te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Maak de opties die worden gebruikt voor extractie van tekstgebieden
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extraheer tekstgebieden die alleen cijfers bevatten uit de linkerbovenhoek van een pagina:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Controleer of extractie van tekstgebieden wordt ondersteund
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Itereer over paginatekstgebieden
    foreach(PageTextArea a in areas)
    {
        // Print een pagina-index, rechthoek en tekstgebiedwaarde:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extraheert tekstgebieden van de documentpagina.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |

### Retourwaarde

Een collectie van [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `null` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voorbeelden

Om tekstgebieden uit een documentpagina te extraheren wordt de volgende methode gebruikt:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Controleer of het document extractie van tekstgebieden ondersteunt
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Haal de documentinformatie op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itereer over pagina's
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Itereer over paginatekstgebieden
        // We negeren null-controle omdat we eerder de ondersteuning van extractie van tekstgebieden hebben gecontroleerd
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Print een rechthoek en tekstgebiedwaarde:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extraheert tekstgebieden van de documentpagina met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoeligheid, enz.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |
| options | PageTextAreaOptions | De opties voor extractie van tekstgebieden. |

### Retourwaarde

Een collectie van [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objecten; `null` als extractie van tekstgebieden niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
