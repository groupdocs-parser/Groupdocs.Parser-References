---
title: GetTables
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Extrait les tableaux du document.
type: docs
weight: 140
url: /fr/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Extrait les tableaux du document.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | PageTableAreaOptions | Les options d'extraction des tables. |

### Return_Value

Une collection de[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objets ; `nul` si l'extraction de tables n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des tableaux de l'ensemble du document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de table
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Création de la disposition des tables
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Création des options d'extraction de table
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extraction des tables du document
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Itération sur les tables
    foreach (PageTableArea t in tables)
    {
        // Itérer sur les lignes
        for (int row = 0; row < t.RowCount; row++)
        {
            // Itérer sur les colonnes
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Récupère la cellule du tableau
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Imprime le texte de la cellule du tableau
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

### Voir également

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Extrait les tableaux de la page du document.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de page de base zéro. |
| options | PageTableAreaOptions | Les options d'extraction des tables. |

### Return_Value

Une collection de[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objets ; `nul` si l'extraction de tables n'est pas prise en charge.

### Exemples

L'exemple suivant montre comment extraire des tableaux de la page du document :

```csharp
// Crée une instance de la classe Parser
using (Parser parser = new Parser(filePath))
{
    // Vérifie si le document prend en charge l'extraction de table
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Création de la disposition des tables
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Création des options d'extraction de table
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Récupère les informations sur le document
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Vérifie si le document contient des pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Itérer sur les pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Imprimer un numéro de page 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraire les tableaux de la page du document
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Itération sur les tables
        foreach (PageTableArea t in tables)
        {
            // Itérer sur les lignes
            for (int row = 0; row < t.RowCount; row++)
            {
                // Itérer sur les colonnes
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Récupère la cellule du tableau
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Imprime le texte de la cellule du tableau
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

### Voir également

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
