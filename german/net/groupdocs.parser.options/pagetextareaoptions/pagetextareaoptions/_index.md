---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions‑Klasse mit der OCR‑Nutzungsoption."
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit der OCR‑Nutzungsoption.

```csharp
public PageTextAreaOptions()
```

### Siehe auch

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit der OCR‑Nutzungsoption.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| useOcr | Boolean | Der Wert, der angibt, ob die OCR‑Funktionalität zum Extrahieren von Textbereichen verwendet wird. |

### Siehe auch

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit der Möglichkeit, OCR‑Optionen festzulegen.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| useOcr | Boolean | Der Wert, der angibt, ob die OCR‑Funktionalität zum Extrahieren von Textbereichen verwendet wird. |
| ocrOptions | OcrOptions | Die zusätzlichen Optionen für die OCR‑Funktionalität. |

### Siehe auch

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit dem regulären Ausdruck. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| expression | String | Der reguläre Ausdruck. |

### Hinweise

Die folgenden Eigenschaften haben Standardwerte:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### Siehe auch

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit dem regulären Ausdruck und dem rechteckigen Bereich. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| expression | String | Der reguläre Ausdruck. |
| Rechteck | Rechteck | Der rechteckige Bereich, der Seitenbereiche enthält. |

### Hinweise

Die folgenden Eigenschaften haben Standardwerte:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit dem regulären Ausdruck, dem rechteckigen Bereich und der Größe des ignorierten Randes. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| expression | String | Der reguläre Ausdruck. |
| Rechteck | Rechteck | Der rechteckige Bereich, der Seitenbereiche enthält. |
| rectangleTolerance | Double | Die Größe des Randes, der beim Erfassen durch den rechteckigen Bereich ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| expression | String | Der reguläre Ausdruck. |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| uniteSegments | Boolean | Der Wert, der angibt, ob Segmente vereinigt sind. |
| ignoreFormatting | Boolean | Der Wert, der angibt, ob die Textformatierung ignoriert wird. |
| Rechteck | Rechteck | Der rechteckige Bereich, der Seitenbereiche enthält. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Initialisiert eine neue Instanz der [`PageTextAreaOptions`](../../pagetextareaoptions)-Klasse mit der Größe des ignorierten Randes.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| expression | String | Der reguläre Ausdruck. |
| matchCase | Boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung eines Textes nicht ignoriert wird. |
| uniteSegments | Boolean | Der Wert, der angibt, ob Segmente vereinigt sind. |
| ignoreFormatting | Boolean | Der Wert, der angibt, ob die Textformatierung ignoriert wird. |
| Rechteck | Rechteck | Der rechteckige Bereich, der Seitenbereiche enthält. |
| rectangleTolerance | Double | Die Größe des Randes, der beim Erfassen durch den rechteckigen Bereich ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
