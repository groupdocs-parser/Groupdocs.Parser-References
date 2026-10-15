---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса BarcodeOptionsgroupdocs.parser.options/barcodeoptions со значениями по умолчанию."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/barcodeoptions/barcodeoptions/
---

## BarcodeOptions() {#constructor}

Инициализирует новый экземпляр класса [`BarcodeOptions`](../../barcodeoptions) со значениями по умолчанию.

```csharp
public BarcodeOptions()
```

### См. также

* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle) {#constructor_1}

Инициализирует новый экземпляр класса [`BarcodeOptions`](../../barcodeoptions) с прямоугольной областью.

```csharp
public BarcodeOptions(Rectangle rectangle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rectangle | Rectangle | Прямоугольная область, содержащая штрихкоды. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(QualityMode, QualityMode, params string[]) {#constructor_3}

Инициализирует новый экземпляр класса [`BarcodeOptions`](../../barcodeoptions) с настройками качества и типами кодов.

```csharp
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, 
    params string[] codeTypes)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageQuality | QualityMode | Качество исходного изображения. |
| barcodeQuality | QualityMode | Качество исходного штрихкода. |
| codeTypes | String[] | Типы штрихкодов для чтения. |

### См. также

* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) {#constructor_2}

Инициализирует новый экземпляр класса [`BarcodeOptions`](../../barcodeoptions).

```csharp
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, 
    float? dimension, bool allowIncorrectBarcodes, params string[] codeTypes)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rectangle | Rectangle | Прямоугольная область, содержащая штрихкоды. |
| imageQuality | QualityMode | Качество исходного изображения. |
| barcodeQuality | QualityMode | Качество исходного штрихкода. |
| dimension | Nullable`1 | Минимальный размер минимального элемента штрихкода. |
| allowIncorrectBarcodes | Boolean | Значение, указывающее, разрешены ли некорректные штрихкоды. |
| codeTypes | String[] | Типы штрихкодов для чтения. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
