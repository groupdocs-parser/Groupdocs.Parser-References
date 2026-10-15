---
title: "المحلل"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "ينشئ مثيلاً جديدًا من الفئة Parsergroupdocs.parser/parser لاستخراج البيانات من عنوان URI."
type: docs
weight: 10
url: /ar/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من عنوان URI.

```csharp
public Parser(Uri uri)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| uri | Uri | عنوان URI الذي يُرسل إليه الطلب. |

### انظر أيضًا

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من عنوان URI مع *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| uri | Uri | عنوان URI الذي يُرسل إليه الطلب. |
| loadOptions | LoadOptions | الخيارات لفتح الملف. |

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من عنوان URI مع *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| uri | Uri | عنوان URI الذي يُرسل إليه الطلب. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### انظر أيضًا

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من عنوان URI مع *loadOptions* و *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| uri | Uri | عنوان URI الذي يُرسل إليه الطلب. |
| loadOptions | LoadOptions | الخيارات لفتح الملف. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من قاعدة بيانات.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الاتصال | DbConnection | اتصال قاعدة البيانات. |

### ملاحظات

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### أمثلة

المثال التالي يوضح كيفية استخراج البيانات من قاعدة بيانات Sqlite:

```csharp
// إنشاء كائن DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// إنشاء مثيل من فئة Parser لاستخراج الجداول من قاعدة البيانات
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
    // التكرار عبر الجداول
    foreach (TocItem i in toc)
    {
        // طباعة اسم الجدول
        Console.WriteLine(i.Text);
        // استخراج محتوى الجدول كنص
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### انظر أيضًا

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من قاعدة بيانات.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الاتصال | DbConnection | اتصال قاعدة البيانات. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### ملاحظات

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### أمثلة

المثال التالي يوضح كيفية استخراج البيانات من قاعدة بيانات Sqlite:

```csharp
// إنشاء كائن DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// إنشاء مثيل من فئة Parser لاستخراج الجداول من قاعدة البيانات
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
    // التكرار عبر الجداول
    foreach (TocItem i in toc)
    {
        // طباعة اسم الجدول
        Console.WriteLine(i.Text);
        // استخراج محتوى الجدول كنص
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### انظر أيضًا

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من خادم بريد إلكتروني بعيد.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الاتصال | EmailConnection | اتصال البريد الإلكتروني. |

### ملاحظات

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### أمثلة

المثال التالي يوضح كيفية استخراج رسائل البريد الإلكتروني من خادم Exchange:

```csharp
// إنشاء كائن الاتصال لبروتوكول Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// إنشاء مثيل من فئة Parser لاستخراج رسائل البريد الإلكتروني من الخادم البعيد
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
 
    // التكرار عبر المرفقات
    foreach (ContainerItem item in emails)
    {
        // إنشاء مثيل من فئة Parser لرسالة البريد الإلكتروني
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

### انظر أيضًا

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

ينشئ مثيلاً جديدًا من الفئة [`Parser`](../../parser) لاستخراج البيانات من خادم بريد إلكتروني بعيد.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الاتصال | EmailConnection | اتصال البريد الإلكتروني. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### ملاحظات

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### أمثلة

المثال التالي يوضح كيفية استخراج رسائل البريد الإلكتروني من خادم Exchange:

```csharp
// إنشاء كائن الاتصال لبروتوكول Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// إنشاء مثيل من فئة Parser لاستخراج رسائل البريد الإلكتروني من الخادم البعيد
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
 
    // التكرار عبر المرفقات
    foreach (ContainerItem item in emails)
    {
        // إنشاء مثيل من فئة Parser لرسالة البريد الإلكتروني
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

### انظر أيضًا

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser).

```csharp
public Parser(string filePath)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| filePath | سلسلة | المسار إلى الملف. |

### ملاحظات

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### أمثلة

المثال التالي يوضح كيفية تحميل المستند من القرص المحلي:

```csharp
// إنشاء مثيل من فئة Parser باستخدام filePath
using (Parser parser = new Parser(filePath))
{
    // استخراج نص إلى القارئ
    using (TextReader reader = parser.GetText())
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا، يكون القارئ null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### انظر أيضًا

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser) باستخدام [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| filePath | سلسلة | المسار إلى الملف. |
| loadOptions | LoadOptions | الخيارات لفتح الملف. |

### ملاحظات

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### أمثلة

كلمة مرور المستند يتم تمريرها عبر فئة LoadOptions:

```csharp
try
{
    // إنشاء مثيل من فئة Parser باستخدام كلمة المرور:
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
    // طباعة الرسالة إذا كانت كلمة المرور غير صحيحة أو فارغة
    Console.WriteLine("Invalid password");
}
```

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser) باستخدام [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| filePath | سلسلة | المسار إلى الملف. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### انظر أيضًا

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser) باستخدام [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) و[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| filePath | سلسلة | المسار إلى الملف. |
| loadOptions | LoadOptions | الخيارات لفتح الملف. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### ملاحظات

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### أمثلة

المثال التالي يوضح كيفية استلام المعلومات عبر واجهة [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // إنشاء مثيل من فئة Logger
    Logger logger = new Logger();
    // إنشاء مثيل من فئة Parser باستخدام إعدادات المحلل
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
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // طباعة رسالة الخطأ
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // طباعة رسالة الحدث
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // طباعة رسالة التحذير
        Console.WriteLine("Warning: " + message);
    }
}
```

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser).

```csharp
public Parser(Stream document)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المستند | Stream | دفق الإدخال المصدر. |

### ملاحظات

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### أمثلة

المثال التالي يوضح كيفية تحميل المستند من الدفق:

```csharp
// إنشاء مثيل من فئة Parser باستخدام الدفق
using (Parser parser = new Parser(stream))
{
    // استخراج نص إلى القارئ
    using (TextReader reader = parser.GetText())
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا، يكون القارئ null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### انظر أيضًا

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser) باستخدام [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المستند | Stream | دفق الإدخال المصدر. |
| loadOptions | LoadOptions | الخيارات لفتح الملف. |

### ملاحظات

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### أمثلة

في بعض الحالات من الضروري تعريف [`FileFormat`](../../../groupdocs.parser.options/fileformat). كلا للحالات الخاصة (قواعد البيانات، خادم البريد) وللكشف عن أنواع الملفات بناءً على المحتوى:

```csharp
// إنشاء نسخة من الفئة Parser لمستند markdown
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
        // تم اكتشاف Markdown؛ يتم طباعة النص بدون الرموز الخاصة
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

كلمة مرور المستند يتم تمريرها عبر فئة [`LoadOptions`](../../../groupdocs.parser.options/loadoptions):

```csharp
try
{
    // إنشاء مثيل من فئة Parser باستخدام كلمة المرور:
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
    // طباعة الرسالة إذا كانت كلمة المرور غير صحيحة أو فارغة
    Console.WriteLine("Invalid password");
}
```

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser) باستخدام [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المستند | Stream | دفق الإدخال المصدر. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### انظر أيضًا

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

يُنشئ مثيلًا جديدًا من فئة [`Parser`](../../parser) باستخدام [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) و[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| المستند | Stream | دفق الإدخال المصدر. |
| loadOptions | LoadOptions | الخيارات لفتح الملف. |
| parserSettings | ParserSettings | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |

### ملاحظات

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### أمثلة

المثال التالي يوضح كيفية استلام المعلومات عبر واجهة [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // إنشاء مثيل من فئة Logger
    Logger logger = new Logger();
    // إنشاء مثيل من فئة Parser باستخدام إعدادات المحلل
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
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // طباعة رسالة الخطأ
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // طباعة رسالة الحدث
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // طباعة رسالة التحذير
        Console.WriteLine("Warning: " + message);
    }
}
```

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
