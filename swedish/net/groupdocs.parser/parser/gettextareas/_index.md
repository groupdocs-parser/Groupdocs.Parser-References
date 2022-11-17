---
title: GetTextAreas
second_title: GroupDocs.Parser för .NET API-referens
description: Extraherar textområden från dokumentet.
type: docs
weight: 160
url: /sv/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Extraherar textområden från dokumentet.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Returvärde

En samling av[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objekt; `null` om extrahering av textområden inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera textområden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exempel

Följande exempel visar hur man extraherar alla textområden från hela dokumentet:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Extrahera textområden
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Kontrollera om extraktion av textområden stöds
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterera över sidtextområden
    foreach(PageTextArea a in areas)
    {
        // Skriv ut ett sidindex, rektangel och textområdesvärde:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Se även

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extraherar textområden från dokumentet med hjälp av anpassningsalternativ (reguljärt uttryck, skiftläge, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | PageTextAreaOptions | Alternativen för extrahering av textområde. |

### Returvärde

En samling av[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objekt; `null` om extrahering av textområden inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera textområden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exempel

Följande exempel visar hur man extraherar endast textområden med siffror från det övre vänstra hörnet:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Skapa alternativen som används för att extrahera textområde
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extrahera textområden som bara innehåller siffror från det övre vänstra hörnet på en sida:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Kontrollera om extraktion av textområden stöds
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterera över sidtextområden
    foreach(PageTextArea a in areas)
    {
        // Skriv ut ett sidindex, rektangel och textområdesvärde:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Se även

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extraherar textområden från dokumentsidan.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |

### Returvärde

En samling av[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objekt; `null` om extrahering av textområden inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera textområden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Exempel

För att extrahera textområden från en dokumentsida används följande metod:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder extraktion av textområden
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Få dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Kontrollera om dokumentet har sidor
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterera över sidor
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Iterera över sidtextområden
        // Vi ignorerar nollkontroll eftersom vi har kontrollerat stöd för extraheringsfunktioner för textområden tidigare
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Skriv ut en rektangel och ett textområdesvärde:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Se även

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extraherar textområden från dokumentsidan med hjälp av anpassningsalternativ (reguljärt uttryck, skiftläge, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |
| options | PageTextAreaOptions | Alternativen för extrahering av textområde. |

### Returvärde

En samling av[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objekt; `null` om extrahering av textområden inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera textområden](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Se även

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
