---
title: "TemplateTable"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "ينشئ مثلاً جديداً من الفئة TemplateTablegroupdocs.parser.templates/templatetable بالاسم بأحرف كبيرة."
type: docs
weight: 10
url: /ar/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

ينشئ مثلاً جديداً من الفئة [`TemplateTable`](../../templatetable) بالاسم بأحرف كبيرة.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| layout | TemplateTableLayout | تخطيط الجدول. |
| name | سلسلة | اسم الجدول. |

### أمثلة

يتم تعيين جدول القالب بواسطة تخطيط الجدول إذا لم يتم اكتشاف الجدول تلقائيًا:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// إنشاء قالب مستند
Template template = new Template(new TemplateItem[] { table });
```

### انظر أيضًا

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

ينشئ مثلاً جديداً من الفئة [`TemplateTable`](../../templatetable) بالاسم بأحرف كبيرة.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| layout | TemplateTableLayout | تخطيط الجدول. |
| name | سلسلة | اسم الجدول. |
| pageWidth | Nullable`1 | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |

### أمثلة

يتم تعيين جدول القالب بواسطة تخطيط الجدول إذا لم يتم اكتشاف الجدول تلقائيًا:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// إنشاء قالب مستند
Template template = new Template(new TemplateItem[] { table });
```

### انظر أيضًا

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

ينشئ مثيلاً جديدًا من الفئة [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| layout | TemplateTableLayout | تخطيط الجدول. |
| name | سلسلة | اسم الجدول. |
| pageWidth | Nullable`1 | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
| useUpperCaseName | Boolean | القيمة التي تشير إلى ما إذا كان `name` يتم تحويله إلى أحرف كبيرة. |

### أمثلة

يتم تعيين جدول القالب بواسطة تخطيط الجدول إذا لم يتم اكتشاف الجدول تلقائيًا:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// إنشاء قالب مستند
Template template = new Template(new TemplateItem[] { table });
```

### انظر أيضًا

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

ينشئ مثيلاً جديدًا من الفئة [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المعلمات | TemplateTableParameters | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
| name | سلسلة | اسم الجدول. |

### أمثلة

إذا تم تعيين جدول القالب بواسطة معلمات الكاشف، يتم اكتشاف الجدول تلقائيًا:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// إنشاء قالب مستند
Template template = new Template(new TemplateItem[] { table });
```

### انظر أيضًا

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

ينشئ مثيلاً جديدًا من الفئة [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المعلمات | TemplateTableParameters | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
| name | سلسلة | اسم الجدول. |
| pageWidth | Nullable`1 | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |

### أمثلة

إذا تم تعيين جدول القالب بواسطة معلمات الكاشف، يتم اكتشاف الجدول تلقائيًا:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// إنشاء قالب مستند
Template template = new Template(new TemplateItem[] { table });
```

### انظر أيضًا

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

ينشئ مثيلاً جديدًا من الفئة [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المعلمات | TemplateTableParameters | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
| name | سلسلة | اسم الجدول. |
| pageWidth | Nullable`1 | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
| useUpperCaseName | Boolean | القيمة التي تشير إلى ما إذا كان `name` يتم تحويله إلى أحرف كبيرة. |

### أمثلة

إذا تم تعيين جدول القالب بواسطة معلمات الكاشف، يتم اكتشاف الجدول تلقائيًا:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// إنشاء قالب مستند
Template template = new Template(new TemplateItem[] { table });
```

### انظر أيضًا

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
