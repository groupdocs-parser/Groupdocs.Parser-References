---
title: "GetBarcodes"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait les codes-barres du document."
type: docs
weight: 70
url: /fr/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Extrait les codes-barres du document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Valeur de retour

Une collection d'objets [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ; `null` si l'extraction des codes-barres n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les codes-barres d'un document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire les codes-barres du document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Itérer sur les codes-barres
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Afficher l'index de la page
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Afficher la valeur du code-barres
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Extrait les codes-barres de la page du document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une collection d'objets [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ; `null` si l'extraction des codes-barres n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les codes-barres d'une page de document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Extraire les codes-barres de la deuxième page du document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Itérer sur les codes-barres
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Afficher l'index de la page
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Afficher la valeur du code-barres
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Extrait les codes-barres du document en utilisant des options de personnalisation.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | BarcodeOptions | Les options pour l'extraction des codes-barres. |

### Valeur de retour

Une collection d'objets [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ; `null` si l'extraction des codes-barres n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les codes-barres du coin supérieur droit.

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Créer les options utilisées pour l'extraction des codes-barres
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extraire les codes-barres du coin supérieur droit.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Itérer sur les codes-barres
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Afficher l'index de la page
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Afficher la valeur du code-barres
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Extrait les codes-barres de la page du document en utilisant des options de personnalisation.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | BarcodeOptions | Les options pour l'extraction des codes-barres. |

### Valeur de retour

Une collection d'objets [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ; `null` si l'extraction des codes-barres n'est pas prise en charge.

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
