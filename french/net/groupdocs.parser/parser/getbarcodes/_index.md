---
title: GetBarcodes
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait les codesbarres du document.
type: docs
weight: 50
url: /fr/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Extrait les codes-barres du document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Return_Value

Une collection de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objets ; `nul` si l'extraction des codes-barres n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des codes-barres d'un document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extrait les codes-barres du document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Itérer sur les codes-barres
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Imprimer l'index de la page
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Imprimer la valeur du code-barres
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Voir également

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Extrait les codes-barres de la page du document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |

### Return_Value

Une collection de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objets ; `nul` si l'extraction des codes-barres n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des codes-barres d'une page de document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extrait les codes-barres de la deuxième page du document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Itérer sur les codes-barres
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Imprimer l'index de la page
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Imprimer la valeur du code-barres
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Voir également

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Extrait les codes-barres du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les codes-barres).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | PageAreaOptions | Les options d'extraction de codes-barres. |

### Return_Value

Une collection de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objets ; `nul` si l'extraction des codes-barres n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les codes-barres du coin supérieur droit.

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Crée les options qui sont utilisées pour l'extraction des codes-barres
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extrait les codes-barres du coin supérieur droit.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Itérer sur les codes-barres
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Imprimer l'index de la page
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Imprimer la valeur du code-barres
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Voir également

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Extrait les codes-barres de la page du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les codes-barres).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | PageAreaOptions | Les options d'extraction de codes-barres. |

### Return_Value

Une collection de[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objets ; `nul` si l'extraction des codes-barres n'est pas prise en charge.

### Voir également

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
