---
title: PageTextArea
second_title: Riferimento API GroupDocs.Parser per .NET
description: Rappresenta unarea di testo della pagina utilizzata per rappresentare un valore di testo nella funzionalità di analisi per modello o modulo di analisi.
type: docs
weight: 140
url: /it/net/groupdocs.parser.data/pagetextarea/
---
## PageTextArea class

Rappresenta un'area di testo della pagina utilizzata per rappresentare un valore di testo nella funzionalità di analisi per modello o modulo di analisi.

```csharp
public sealed class PageTextArea : PageArea
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | Inizializza una nuova istanza di[`PageTextArea`](../pagetextarea) classe. |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | Inizializza una nuova istanza di[`PageTextArea`](../pagetextarea) classe. |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | Inizializza una nuova istanza di[`PageTextArea`](../pagetextarea) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | Ottiene la raccolta delle aree della pagina di testo figlio. |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | Ottiene la linea di base. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Ottiene le informazioni sulla pagina del documento come l'indice della pagina e le dimensioni della pagina. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Ottiene l'area rettangolare. |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | Ottiene il testo. |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | Ottiene lo stile del testo come la dimensione del carattere, il nome del carattere e così via. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | Converte il valore di questa istanza inString . |

### Osservazioni

Un'istanza di[`PageTextArea`](../pagetextarea) class viene utilizzata come valore di ritorno dei seguenti metodi:

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

Anche un'istanza di[`PageTextArea`](../pagetextarea) la classe viene utilizzata come valore di[`PageArea`](../fielddata/pagearea) proprietà.

Vedi gli esempi di utilizzo qui.

L'area di testo può essere singola o composita. Nel primo caso contiene un testo delimitato da un'area rettangolare. Nel secondo caso contiene altre aree di testo; le proprietà del testo e della tabella sono calcolate dalle aree di testo figlio.

### Guarda anche

* class [PageArea](../pagearea)
* spazio dei nomi [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assemblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->