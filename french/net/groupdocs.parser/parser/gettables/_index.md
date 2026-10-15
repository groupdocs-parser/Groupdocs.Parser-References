---
title: "GetTables"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Extrait les tableaux du document."
type: docs
weight: 170
url: /fr/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Extrait les tableaux du document.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | PageTableAreaOptions | Les options pour l'extraction des tables. |

### Valeur de retour

Une collection d'objets [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ; `null` si l'extraction des tables n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les tables du document complet :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de tables
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Créer la mise en page des tables
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Créer les options pour l'extraction de tables
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extraire les tables du document
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Itérer sur les tables
    foreach (PageTableArea t in tables)
    {
        // Parcourir les lignes
        for (int row = 0; row < t.RowCount; row++)
        {
            // Parcourir les colonnes
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Obtenir la cellule du tableau
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Imprimer le texte de la cellule du tableau
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Extrait les tableaux de la page du document.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |
| options | PageTableAreaOptions | Les options pour l'extraction des tables. |

### Valeur de retour

Une collection d'objets [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ; `null` si l'extraction des tables n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les tables de la page du document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de tables
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Créer la mise en page des tables
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Créer les options pour l'extraction de tables
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Obtenir les informations du document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifier si le document possède des pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Parcourir les pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraire les tables de la page du document
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Itérer sur les tables
        foreach (PageTableArea t in tables)
        {
            // Parcourir les lignes
            for (int row = 0; row < t.RowCount; row++)
            {
                // Parcourir les colonnes
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Obtenir la cellule du tableau
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Imprimer le texte de la cellule du tableau
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Extrait les tableaux du document.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Valeur de retour

Une collection d'objets [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ; `null` si l'extraction des tables n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les tables du document complet :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de tables
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Extraire les tables du document
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Itérer sur les tables
    foreach (PageTableArea t in tables)
    {
        // Parcourir les lignes
        for (int row = 0; row < t.RowCount; row++)
        {
            // Parcourir les colonnes
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Obtenir la cellule du tableau
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Imprimer le texte de la cellule du tableau
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Extrait les tableaux de la page du document.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page basé sur zéro. |

### Valeur de retour

Une collection d'objets [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ; `null` si l'extraction des tables n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire les tables de la page du document :

```csharp
// Créez une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifier si le document prend en charge l'extraction de tables
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Obtenir les informations du document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifier si le document possède des pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Parcourir les pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Afficher le numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraire les tables de la page du document
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Itérer sur les tables
        foreach (PageTableArea t in tables)
        {
            // Parcourir les lignes
            for (int row = 0; row < t.RowCount; row++)
            {
                // Parcourir les colonnes
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Obtenir la cellule du tableau
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Imprimer le texte de la cellule du tableau
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
