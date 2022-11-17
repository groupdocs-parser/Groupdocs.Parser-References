---
title: TemplateField
second_title: Riferimento API GroupDocs.Parser per .NET
description: Fornisce il campo di testo del modello.
type: docs
weight: 620
url: /it/net/groupdocs.parser.templates/templatefield/
---
## TemplateField class

Fornisce il campo di testo del modello.

```csharp
public sealed class TemplateField : TemplateItem
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | Inizializza una nuova istanza di[`TemplateField`](../templatefield) classe. |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, int?) | Inizializza una nuova istanza di[`TemplateField`](../templatefield) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Ottiene il nome dell'elemento del modello. |
| [PageIndex](../../groupdocs.parser.templates/templateitem/pageindex) { get; } | Ottiene l'indice della pagina dell'elemento del modello. |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | Ottiene il valore che descrive come trovare il campo del modello nella pagina del documento. |

### Osservazioni

I campi di testo sono definiti dalla sua posizione nella pagina. Esistono tre modi per definire un campo di testo:

* [`Utilizzando l'area rettangolare`](../templatefixedposition)
* [`Usando l'espressione regolare`](../templateregexposition)
* [`Utilizzando il campo collegato`](../templatelinkedposition)

### Guarda anche

* class [TemplateItem](../templateitem)
* spazio dei nomi [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assemblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->