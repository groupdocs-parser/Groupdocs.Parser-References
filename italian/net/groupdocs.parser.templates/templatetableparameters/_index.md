---
title: TemplateTableParameters
second_title: Riferimento API GroupDocs.Parser per .NET
description: Fornisce i parametri per gli algoritmi di rilevamento della tabella.
type: docs
weight: 710
url: /it/net/groupdocs.parser.templates/templatetableparameters/
---
## TemplateTableParameters class

Fornisce i parametri per gli algoritmi di rilevamento della tabella.

```csharp
public sealed class TemplateTableParameters
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Inizializza una nuova istanza di[`TemplateTableParameters`](../templatetableparameters) classe. |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Inizializza una nuova istanza di[`TemplateTableParameters`](../templatetableparameters) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Ottiene il valore che indica se la tabella ha celle unite. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Ottiene il numero minimo di colonne della tabella. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Ottiene il numero minimo di righe della tabella. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Ottiene lo spazio minimo tra le colonne della tabella. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Ottiene l'area rettangolare che contiene la tabella. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Ottiene i separatori delle colonne della tabella. |

### Osservazioni

Esistono due algoritmi per rilevare una tabella:

* Consente di rilevare una tabella nell'area rettangolare con colonne impostate. Questo algoritmo è utile per tabelle semplici (senza colonne unite) e fornisce un rilevamento più accurato.
* Consente di rilevare una tabella in qualsiasi punto della pagina. Questo è un algoritmo più complesso. Può rilevare le tabelle in qualsiasi punto della pagina. Parametri aggiuntivi aiutano a rilevare una tabella in modo più corretto.

In alcuni casi in cui gli algoritmi non sono in grado di rilevare una tabella o lo fanno in modo non accurato [`TemplateTableLayout`](../templatetablelayout) viene utilizzata la classe.

### Guarda anche

* spazio dei nomi [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assemblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->