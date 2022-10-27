---
title: SearchOptions
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Inicializa una nueva instancia delSearchOptionsgroupdocs.parser.options/searchoptions clase.
type: docs
weight: 10
url: /es/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Inicializa una nueva instancia del[`SearchOptions`](../../searchoptions) clase.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| matchCase | Boolean | El valor que indica si un caso de texto no se ignora. |
| matchWholeWord | Boolean | El valor que indica si la búsqueda de texto está limitada por una palabra completa. |
| useRegularExpression | Boolean | El valor que indica si se utiliza una expresión regular. |
| searchByPages | Boolean | El valor que indica si la búsqueda se realiza por páginas. |
| leftHighlightOptions | HighlightOptions | Las opciones para el resaltado izquierdo. |
| rightHighlightOptions | HighlightOptions | Las opciones para el resaltado derecho. |

### Ver también

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* espacio de nombres [GroupDocs.Parser.Options](../../searchoptions)
* asamblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Inicializa una nueva instancia del[`SearchOptions`](../../searchoptions) clase que se utiliza para buscar con las opciones de resaltado para la extracción de resaltado izquierdo y derecho.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| matchCase | Boolean | El valor que indica si un caso de texto no se ignora. |
| matchWholeWord | Boolean | El valor que indica si la búsqueda de texto está limitada por una palabra completa. |
| useRegularExpression | Boolean | El valor que indica si se utiliza una expresión regular. |
| leftHighlightOptions | HighlightOptions | Las opciones para el resaltado izquierdo. |
| rightHighlightOptions | HighlightOptions | Las opciones para el resaltado derecho. |

### Ver también

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* espacio de nombres [GroupDocs.Parser.Options](../../searchoptions)
* asamblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Inicializa una nueva instancia del[`SearchOptions`](../../searchoptions) clase que se utiliza para buscar con las mismas opciones de resaltado para la extracción de resaltado izquierdo y derecho.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| matchCase | Boolean | El valor que indica si un caso de texto no se ignora. |
| matchWholeWord | Boolean | El valor que indica si la búsqueda de texto está limitada por una palabra completa. |
| useRegularExpression | Boolean | El valor que indica si se utiliza una expresión regular. |
| highlightOptions | HighlightOptions | Las opciones para ambos aspectos destacados. |

### Ver también

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* espacio de nombres [GroupDocs.Parser.Options](../../searchoptions)
* asamblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Inicializa una nueva instancia del[`SearchOptions`](../../searchoptions) clase que se utiliza para buscar sin extracción de resaltado.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| matchCase | Boolean | El valor que indica si un caso de texto no se ignora. |
| matchWholeWord | Boolean | El valor que indica si la búsqueda de texto está limitada por una palabra completa. |
| useRegularExpression | Boolean | El valor que indica si se utiliza una expresión regular. |

### Ver también

* class [SearchOptions](../../searchoptions)
* espacio de nombres [GroupDocs.Parser.Options](../../searchoptions)
* asamblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Inicializa una nueva instancia del[`SearchOptions`](../../searchoptions) clase que se utiliza para buscar por páginas y sin extracción de resaltado.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| matchCase | Boolean | El valor que indica si un caso de texto no se ignora. |
| matchWholeWord | Boolean | El valor que indica si la búsqueda de texto está limitada por una palabra completa. |
| useRegularExpression | Boolean | El valor que indica si se utiliza una expresión regular. |
| searchByPages | Boolean | El valor que indica si la búsqueda se realiza por páginas. |

### Ver también

* class [SearchOptions](../../searchoptions)
* espacio de nombres [GroupDocs.Parser.Options](../../searchoptions)
* asamblea [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Inicializa una nueva instancia del[`SearchOptions`](../../searchoptions) clase con valores predeterminados. Ver comentarios para más detalles.

```csharp
public SearchOptions()
```

### Observaciones

Las siguientes propiedades tienen valores predeterminados:

**[`MatchCase`](../matchcase)**

`falso`

**[`MatchWholeWord`](../matchwholeword)**

`falso`

**[`UseRegularExpression`](../useregularexpression)**

`falso`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`nulo`

**[`RightHighlightOptions`](../righthighlightoptions)**

`nulo`

### Ver también

* class [SearchOptions](../../searchoptions)
* espacio de nombres [GroupDocs.Parser.Options](../../searchoptions)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
