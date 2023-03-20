---
title: SearchOptions
second_title: GroupDocs.Parser لمرجع .NET API
description: يقوم بتهيئة مثيل جديد لملفSearchOptionsgroupdocs.parser.options/searchoptions فئة .
type: docs
weight: 10
url: /ar/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

يقوم بتهيئة مثيل جديد لملف[`SearchOptions`](../../searchoptions) فئة .

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى عدم تجاهل حالة النص. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث عن نص مقيدًا بكلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى استخدام تعبير عادي. |
| searchByPages | Boolean | القيمة التي تشير إلى ما إذا كان البحث يتم بواسطة الصفحات أم لا. |
| leftHighlightOptions | HighlightOptions | خيارات التمييز الأيسر. |
| rightHighlightOptions | HighlightOptions | خيارات التمييز الصحيح. |

### أنظر أيضا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* مساحة الاسم [GroupDocs.Parser.Options](../../searchoptions)
* المجسم [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

يقوم بتهيئة مثيل جديد لملف[`SearchOptions`](../../searchoptions) فئة تستخدم للبحث مع خيارات التمييز لاستخراج التمييز الأيمن والأيسر.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى عدم تجاهل حالة النص. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث عن نص مقيدًا بكلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى استخدام تعبير عادي. |
| leftHighlightOptions | HighlightOptions | خيارات التمييز الأيسر. |
| rightHighlightOptions | HighlightOptions | خيارات التمييز الصحيح. |

### أنظر أيضا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* مساحة الاسم [GroupDocs.Parser.Options](../../searchoptions)
* المجسم [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

يقوم بتهيئة مثيل جديد لملف[`SearchOptions`](../../searchoptions) الفئة التي تُستخدم للبحث مع نفس خيارات التمييز لاستخراج التمييز الأيمن والأيسر.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى عدم تجاهل حالة النص. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث عن نص مقيدًا بكلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى استخدام تعبير عادي. |
| highlightOptions | HighlightOptions | الخيارات لكل من الإبرازات. |

### أنظر أيضا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* مساحة الاسم [GroupDocs.Parser.Options](../../searchoptions)
* المجسم [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`SearchOptions`](../../searchoptions) الفئة التي تستخدم للبحث دون تمييز الاستخراج.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى عدم تجاهل حالة النص. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث عن نص مقيدًا بكلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى استخدام تعبير عادي. |

### أنظر أيضا

* class [SearchOptions](../../searchoptions)
* مساحة الاسم [GroupDocs.Parser.Options](../../searchoptions)
* المجسم [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`SearchOptions`](../../searchoptions)الفئة التي يتم استخدامها للبحث عن طريق الصفحات و دون تمييز الاستخراج.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى عدم تجاهل حالة النص. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث عن نص مقيدًا بكلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى استخدام تعبير عادي. |
| searchByPages | Boolean | القيمة التي تشير إلى ما إذا كان البحث يتم بواسطة الصفحات أم لا. |

### أنظر أيضا

* class [SearchOptions](../../searchoptions)
* مساحة الاسم [GroupDocs.Parser.Options](../../searchoptions)
* المجسم [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`SearchOptions`](../../searchoptions) فئة مع القيم الافتراضية. انظر الملاحظات للحصول على التفاصيل.

```csharp
public SearchOptions()
```

### ملاحظات

الخصائص التالية لها قيم افتراضية:

**[`MatchCase`](../matchcase)**

`خطأ شنيع`

**[`MatchWholeWord`](../matchwholeword)**

`خطأ شنيع`

**[`UseRegularExpression`](../useregularexpression)**

`خطأ شنيع`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`باطل`

**[`RightHighlightOptions`](../righthighlightoptions)**

`باطل`

### أنظر أيضا

* class [SearchOptions](../../searchoptions)
* مساحة الاسم [GroupDocs.Parser.Options](../../searchoptions)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
