---
title: Parser
second_title: GroupDocs.Parser لمرجع .NET API
description: يقوم بتهيئة مثيل جديد لملفParsergroupdocs.parser/parser فئة لاستخراج البيانات من قاعدة بيانات.
type: docs
weight: 10
url: /ar/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة لاستخراج البيانات من قاعدة بيانات.

```csharp
public Parser(DbConnection connection)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| connection | DbConnection | اتصال قاعدة البيانات. |

### ملاحظات

**يتعلم أكثر:**

* [استخراج البيانات من قواعد البيانات](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### أمثلة

يوضح المثال التالي كيفية استخراج البيانات من قاعدة بيانات Sqlite:

```csharp
// إنشاء كائن DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// إنشاء مثيل لفئة Parser لاستخراج الجداول من قاعدة البيانات
using (Parser parser = new Parser(connection))
{
    // تحقق مما إذا كان استخراج النص مدعومًا
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // تحقق مما إذا كان استخراج toc مدعومًا
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // احصل على قائمة الجداول
    IEnumerable<TocItem> toc = parser.GetToc();
    // تكرار على الطاولات
    foreach (TocItem i in toc)
    {
        // اطبع اسم الجدول
        Console.WriteLine(i.Text);
        // استخراج محتوى جدول كنص
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### أنظر أيضا

* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة لاستخراج البيانات من قاعدة بيانات.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| connection | DbConnection | اتصال قاعدة البيانات. |
| parserSettings | ParserSettings | إعدادات المحلل اللغوي المستخدمة لتخصيص استخراج البيانات. |

### ملاحظات

**يتعلم أكثر:**

* [استخراج البيانات من قواعد البيانات](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [تسجيل](https://docs.groupdocs.com/display/parsernet/Logging)

### أمثلة

يوضح المثال التالي كيفية استخراج البيانات من قاعدة بيانات Sqlite:

```csharp
// إنشاء كائن DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// إنشاء مثيل لفئة Parser لاستخراج الجداول من قاعدة البيانات
using (Parser parser = new Parser(connection))
{
    // تحقق مما إذا كان استخراج النص مدعومًا
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // تحقق مما إذا كان استخراج toc مدعومًا
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // احصل على قائمة الجداول
    IEnumerable<TocItem> toc = parser.GetToc();
    // تكرار على الطاولات
    foreach (TocItem i in toc)
    {
        // اطبع اسم الجدول
        Console.WriteLine(i.Text);
        // استخراج محتوى جدول كنص
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### أنظر أيضا

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة لاستخراج البيانات من خادم بريد إلكتروني بعيد.

```csharp
public Parser(EmailConnection connection)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| connection | EmailConnection | اتصال البريد الإلكتروني. |

### ملاحظات

**يتعلم أكثر:**

* [استخراج رسائل البريد الإلكتروني من الخادم البعيد عبر بروتوكولات POP أو IMAP أو Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### أمثلة

يوضح المثال التالي كيفية استخراج رسائل البريد الإلكتروني من خادم Exchange:

```csharp
// إنشاء كائن الاتصال لبروتوكول خدمات ويب Exchange 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx "،
    "email@server",
    "password");
 
// إنشاء مثيل لفئة المحلل اللغوي لاستخراج رسائل البريد الإلكتروني من الخادم البعيد
using (Parser parser = new Parser(connection))
{
    // تحقق مما إذا كان استخراج الحاوية مدعومًا
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// استخراج رسائل البريد الإلكتروني من الخادم
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // كرر عبر المرفقات
    foreach (ContainerItem item in emails)
    {
        // إنشاء مثيل لفئة Parser لرسالة البريد الإلكتروني
        using (Parser emailParser = item.OpenParser())
        {
            // استخراج نص البريد الإلكتروني
            using (TextReader reader = emailParser.GetText())
            {
                // طباعة نص البريد الإلكتروني
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### أنظر أيضا

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة لاستخراج البيانات من خادم بريد إلكتروني بعيد.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| connection | EmailConnection | اتصال البريد الإلكتروني. |
| parserSettings | ParserSettings | إعدادات المحلل اللغوي المستخدمة لتخصيص استخراج البيانات. |

### ملاحظات

**يتعلم أكثر:**

* [استخراج رسائل البريد الإلكتروني من الخادم البعيد عبر بروتوكولات POP أو IMAP أو Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [تسجيل](https://docs.groupdocs.com/display/parsernet/Logging)

### أمثلة

يوضح المثال التالي كيفية استخراج رسائل البريد الإلكتروني من خادم Exchange:

```csharp
// إنشاء كائن الاتصال لبروتوكول خدمات ويب Exchange 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx "،
    "email@server",
    "password");
 
// إنشاء مثيل لفئة المحلل اللغوي لاستخراج رسائل البريد الإلكتروني من الخادم البعيد
using (Parser parser = new Parser(connection))
{
    // تحقق مما إذا كان استخراج الحاوية مدعومًا
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// استخراج رسائل البريد الإلكتروني من الخادم
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // كرر عبر المرفقات
    foreach (ContainerItem item in emails)
    {
        // إنشاء مثيل لفئة Parser لرسالة البريد الإلكتروني
        using (Parser emailParser = item.OpenParser())
        {
            // استخراج نص البريد الإلكتروني
            using (TextReader reader = emailParser.GetText())
            {
                // طباعة نص البريد الإلكتروني
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### أنظر أيضا

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_7}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة .

```csharp
public Parser(string filePath)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |

### ملاحظات

**يتعلم أكثر:**

* [تحميل المستند من القرص المحلي](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### أمثلة

يوضح المثال التالي كيفية تحميل المستند من القرص المحلي:

```csharp
// إنشاء مثيل لفئة Parser باستخدام filePath
using (Parser parser = new Parser(filePath))
{
    // استخراج نص في القارئ
    using (TextReader reader = parser.GetText())
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا ، يكون القارئ فارغًا
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### أنظر أيضا

* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_8}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة مع[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| loadOptions | LoadOptions | خيارات فتح الملف. |

### ملاحظات

**يتعلم أكثر:**

* [تحميل تنسيقات ملفات محددة](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [تحميل المستندات المحمية بكلمة مرور](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [تحميل المستند من القرص المحلي](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### أمثلة

يتم تمرير كلمة مرور المستند من خلال فئة LoadOptions:

```csharp
try
{
    // إنشاء مثيل لفئة Parser باستخدام كلمة المرور:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // تحقق مما إذا كان استخراج النص مدعومًا
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // طباعة نص المستند
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // اطبع الرسالة إذا كانت كلمة المرور غير صحيحة أو فارغة
    Console.WriteLine("Invalid password");
}
```

### أنظر أيضا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_9}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة مع[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) و[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| loadOptions | LoadOptions | خيارات فتح الملف. |
| parserSettings | ParserSettings | إعدادات المحلل اللغوي المستخدمة لتخصيص استخراج البيانات. |

### ملاحظات

**يتعلم أكثر:**

* [تحميل تنسيقات ملفات محددة](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [تحميل المستندات المحمية بكلمة مرور](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [تسجيل](https://docs.groupdocs.com/display/parsernet/Logging)
* [تحميل المستند من القرص المحلي](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### أمثلة

يوضح المثال التالي كيفية تلقي المعلومات عبر[`ILogger`](../../../groupdocs.parser.options/ilogger) واجهه المستخدم:

```csharp
// محاولة
{
    // إنشاء مثيل لفئة المسجل
    Logger logger = new Logger();
    // إنشاء مثيل لفئة المحلل اللغوي باستخدام إعدادات المحلل اللغوي
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // تحقق مما إذا كان استخراج النص مدعومًا
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // طباعة نص المستند
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // تجاهل الاستثناء
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // طباعة رسالة خطأ
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // طباعة رسالة الحدث
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // طباعة رسالة تحذير
        Console.WriteLine("Warning: " + message);
    }
}
```

### أنظر أيضا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة .

```csharp
public Parser(Stream document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| document | Stream | دفق إدخال المصدر. |

### ملاحظات

**يتعلم أكثر:**

* [تحميل المستند من الدفق](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### أمثلة

يوضح المثال التالي كيفية تحميل المستند من الدفق:

```csharp
// إنشاء مثيل لفئة Parser مع الدفق
using (Parser parser = new Parser(stream))
{
    // استخراج نص في القارئ
    using (TextReader reader = parser.GetText())
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا ، يكون القارئ فارغًا
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### أنظر أيضا

* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة مع[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| document | Stream | دفق إدخال المصدر. |
| loadOptions | LoadOptions | خيارات فتح الملف. |

### ملاحظات

**يتعلم أكثر:**

* [تحميل تنسيقات ملفات محددة](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [تحميل المستندات المحمية بكلمة مرور](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [تحميل المستند من الدفق](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### أمثلة

في بعض الحالات ، من الضروري تحديد[`FileFormat`](../../../groupdocs.parser.options/fileformat). لكل من الحالات الخاصة (قواعد البيانات وخادم البريد الإلكتروني) وللكشف عن أنواع الملفات حسب المحتوى:

تم تمرير كلمة مرور المستند[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) صف دراسي:

```csharp
// إنشاء مثيل لفئة Parser لمستند markdown
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // تحقق مما إذا كان استخراج النص مدعومًا
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // طباعة نص المستند
        // تم الكشف عن تخفيض السعر ; تتم طباعة النص بدون رموز خاصة
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // إنشاء مثيل لفئة Parser باستخدام كلمة المرور:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // تحقق مما إذا كان استخراج النص مدعومًا
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // طباعة نص المستند
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // اطبع الرسالة إذا كانت كلمة المرور غير صحيحة أو فارغة
    Console.WriteLine("Invalid password");
}
```

### أنظر أيضا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

يقوم بتهيئة مثيل جديد لملف[`Parser`](../../parser) فئة مع[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) و[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| document | Stream | دفق إدخال المصدر. |
| loadOptions | LoadOptions | خيارات فتح الملف. |
| parserSettings | ParserSettings | إعدادات المحلل اللغوي المستخدمة لتخصيص استخراج البيانات. |

### ملاحظات

**يتعلم أكثر:**

* [تحميل تنسيقات ملفات محددة](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [تحميل المستندات المحمية بكلمة مرور](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [تحميل المستند من الدفق](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [تسجيل](https://docs.groupdocs.com/display/parsernet/Logging)

### أمثلة

يوضح المثال التالي كيفية تلقي المعلومات عبر[`ILogger`](../../../groupdocs.parser.options/ilogger) واجهه المستخدم:

```csharp
// محاولة
{
    // إنشاء مثيل لفئة المسجل
    Logger logger = new Logger();
    // إنشاء مثيل لفئة المحلل اللغوي باستخدام إعدادات المحلل اللغوي
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // تحقق مما إذا كان استخراج النص مدعومًا
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // طباعة نص المستند
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // تجاهل الاستثناء
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // طباعة رسالة خطأ
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // طباعة رسالة الحدث
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // طباعة رسالة تحذير
        Console.WriteLine("Warning: " + message);
    }
}
```

### أنظر أيضا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
