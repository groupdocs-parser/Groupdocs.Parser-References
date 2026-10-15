---
title: "पार्सर"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "टेक्स्ट इमेज कंटेनर निष्कर्षण और पार्सिंग कार्यक्षमता को नियंत्रित करने वाली मुख्य क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 30
url: /hi/net/groupdocs.parser/parser/
---

## Parser class

पाठ, छवियों, कंटेनर निष्कर्षण और पार्सिंग कार्यक्षमता को नियंत्रित करने वाली मुख्य क्लास को दर्शाता है।

```csharp
public sealed class Parser : IDisposable
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि डेटाबेस से डेटा निकाला जा सके। |
| [Parser](parser#constructor)(EmailConnection) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि रिमोट ईमेल सर्वर से डेटा निकाला जा सके। |
| [Parser](parser#constructor_4)(Stream) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [Parser](parser#constructor_8)(string) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [Parser](parser#constructor_12)(Uri) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि URI से डेटा निकाला जा सके। |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि डेटाबेस से डेटा निकाला जा सके। |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि रिमोट ईमेल सर्वर से डेटा निकाला जा सके। |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है [`LoadOptions`](../../groupdocs.parser.options/loadoptions) के साथ। |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है [`ParserSettings`](../../groupdocs.parser.options/parsersettings) के साथ। |
| [Parser](parser#constructor_9)(string, LoadOptions) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है [`LoadOptions`](../../groupdocs.parser.options/loadoptions) के साथ। |
| [Parser](parser#constructor_11)(string, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है [`ParserSettings`](../../groupdocs.parser.options/parsersettings) के साथ। |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि URI से डेटा निकाला जा सके *loadOptions* के साथ। |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि URI से डेटा निकाला जा सके *parserSettings* के साथ। |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है [`LoadOptions`](../../groupdocs.parser.options/loadoptions) और [`ParserSettings`](../../groupdocs.parser.options/parsersettings) के साथ। |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है [`LoadOptions`](../../groupdocs.parser.options/loadoptions) और [`ParserSettings`](../../groupdocs.parser.options/parsersettings) के साथ। |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | `[`Parser`](../parser)` क्लास का नया इंस्टेंस प्रारंभ करता है ताकि URI से डेटा निकाला जा सके *loadOptions* और *parserSettings* के साथ। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | समर्थित सुविधाएँ प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | अनुप्रयोग-परिभाषित कार्य करता है जो अनमैनेज्ड संसाधनों को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित हैं। |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | टेम्पलेट की स्थिति और स्केल के स्वचालित समायोजन के लिए फ़ील्ड उत्पन्न करता है। |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | पृष्ठों का पूर्वावलोकन प्राप्त करें। |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | दस्तावेज़ से एनोटेशन निकालता है। नोट करें कि वर्तमान में केवल PDF फ़ॉर्मेट समर्थित है। |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | दस्तावेज़ पृष्ठ से एनोटेशन निकालता है। नोट करें कि वर्तमान में केवल PDF फ़ॉर्मेट समर्थित है। |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | दस्तावेज़ से बारकोड निकालता है। |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ से बारकोड निकालता है। |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | दस्तावेज़ पृष्ठ से बारकोड निकालता है। |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से बारकोड निकालता है। |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | संलग्नक, ZIP अभिलेख आदि वाले फ़ॉर्मेट के साथ काम करने के लिए दस्तावेज़ से एक कंटेनर ऑब्जेक्ट निकालता है। |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है। |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | दस्तावेज़ से फ़ॉर्मेटेड टेक्स्ट निकालता है। |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | दस्तावेज़ पृष्ठ से फ़ॉर्मेटेड टेक्स्ट निकालता है। |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | दस्तावेज़ से हाइलाइट निकालता है। |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | दस्तावेज़ से हाइपरलिंक निकालता है। |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है। |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए)। |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए)। |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | दस्तावेज़ से छवियां निकालता है। |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | दस्तावेज़ पृष्ठ से छवियां निकालता है। |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ से छवियां निकालता है (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए)। |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से छवियां निकालता है (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए)। |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | दस्तावेज़ से मेटाडेटा निकालता है। |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है। |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है। |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | दस्तावेज़ से संरचित टेक्स्ट निकालता है। |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | दस्तावेज़ से तालिकाएं निकालता है। |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | दस्तावेज़ पृष्ठ से तालिकाएँ निकालता है। |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | दस्तावेज़ से तालिकाएं निकालता है। |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | दस्तावेज़ पृष्ठ से तालिकाएँ निकालता है। |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | दस्तावेज़ से पाठ निकालता है। |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | दस्तावेज़ पृष्ठ से पाठ निकालता है। |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | दस्तावेज़ से पाठ पृष्ठ निकालता है, पाठ विकल्पों का उपयोग करके (कच्चा तेज़ पाठ निष्कर्षण मोड सक्षम करने के लिए)। |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | दस्तावेज़ पृष्ठ से पाठ निकालता है, पाठ विकल्पों का उपयोग करके (कच्चा तेज़ पाठ निष्कर्षण मोड सक्षम करने के लिए)। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | दस्तावेज़ से पाठ क्षेत्रों को निकालता है। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | दस्तावेज़ पृष्ठ से पाठ क्षेत्रों को निकालता है। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | दस्तावेज़ से पाठ क्षेत्रों को निकालता है, अनुकूलन विकल्पों का उपयोग करके (रेगुलर एक्सप्रेशन, केस मिलान, आदि)। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | दस्तावेज़ पृष्ठ से पाठ क्षेत्रों को निकालता है, अनुकूलन विकल्पों का उपयोग करके (रेगुलर एक्सप्रेशन, केस मिलान, आदि)। |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | दस्तावेज़ से सामग्री तालिका निकालता है। |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | वर्कशीट कोशिकाएँ निकालता है। |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | वर्कशीट कोशिकाएँ निकालता है, अनुकूलन विकल्पों का उपयोग करके। |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | स्प्रेडशीट में सभी वर्कशीट्स की जानकारी निकालता है। |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | वर्कशीट की जानकारी निकालता है। |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | उपयोगकर्ता-निर्मित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है। |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | उपयोगकर्ता-निर्मित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है, अनुकूलन विकल्पों का उपयोग करके। |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | प्रदान किए गए संग्रह से सबसे उपयुक्त टेम्पलेट चुनता है और फिर चयनित टेम्पलेट के विरुद्ध दस्तावेज़ को पार्स करता है। |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | दस्तावेज़ फ़ॉर्म को पार्स करता है। |
| [Search](../../groupdocs.parser/parser/search#search)(string) | दस्तावेज़ में एक *keyword* खोजता है। |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | दस्तावेज़ में एक *keyword* खोजता है, खोज विकल्पों का उपयोग करके (रेगुलर एक्सप्रेशन, केस मिलान, आदि)। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |

### संबंधित देखें

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
