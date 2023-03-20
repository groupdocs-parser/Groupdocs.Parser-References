---
title: Parser
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: मुख्य वर्ग क प्रतनधत्व करत है ज पठ छवयं कंटेनर नष्कर्षण और पर्संग कर्यक्षमत क नयंत्रत करत है
type: docs
weight: 640
url: /hi/net/groupdocs.parser/parser/
---
## Parser class

मुख्य वर्ग का प्रतिनिधित्व करता है जो पाठ, छवियों, कंटेनर निष्कर्षण और पार्सिंग कार्यक्षमता को नियंत्रित करता है।

```csharp
public sealed class Parser : IDisposable
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) वर्ग एक डेटाबेस से डेटा निकालने के लिए। |
| [Parser](parser#constructor)(EmailConnection) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) वर्ग एक दूरस्थ ईमेल सर्वर से डेटा निकालने के लिए। |
| [Parser](parser#constructor_4)(Stream) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) वर्ग. |
| [Parser](parser#constructor_8)(string) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) वर्ग. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) वर्ग एक डेटाबेस से डेटा निकालने के लिए। |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) वर्ग एक दूरस्थ ईमेल सर्वर से डेटा निकालने के लिए। |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) के साथ वर्ग[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) के साथ वर्ग[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) के साथ वर्ग[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) के साथ वर्ग[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) के साथ वर्ग[`LoadOptions`](../../groupdocs.parser.options/loadoptions) और[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | का एक नया उदाहरण प्रारंभ करता है[`Parser`](../parser) के साथ वर्ग[`LoadOptions`](../../groupdocs.parser.options/loadoptions) और[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## गुण

| नाम | विवरण |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | समर्थित सुविधाएँ प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | अप्रबंधित संसाधनों को मुक्त करने, जारी करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्य करता है। |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | पृष्ठों का पूर्वावलोकन प्राप्त करें. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | दस्तावेज़ से बारकोड निकालता है। |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | दस्तावेज़ पृष्ठ से बारकोड निकालता है. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ से बारकोड निकालता है (बारकोड वाले आयताकार क्षेत्र को सेट करने के लिए) |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से बारकोड निकालता है (बारकोड वाले आयताकार क्षेत्र को सेट करने के लिए) |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | दस्तावेज़ से एक कंटेनर ऑब्जेक्ट को निकालता है ताकि अटैचमेंट, ज़िप संग्रह आदि वाले प्रारूपों के साथ काम किया जा सके. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है। |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | दस्तावेज़ से एक स्वरूपित पाठ निकालता है। |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | दस्तावेज़ पृष्ठ से एक स्वरूपित पाठ निकालता है। |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | दस्तावेज़ से हाइलाइट निकालता है. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | दस्तावेज़ से हाइपरलिंक निकालता है। |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए) |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए) |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | दस्तावेज़ से छवियों को निकालता है। |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | दस्तावेज़ पृष्ठ से छवियां निकालता है. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ से छवियों को निकालता है (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए) |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से छवियां निकालता है (आयताकार क्षेत्र सेट करने के लिए जिसमें चित्र शामिल हैं) |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | दस्तावेज़ से मेटाडेटा निकालता है। |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | दस्तावेज़ से एक संरचित पाठ निकालता है। |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | दस्तावेज़ से तालिकाएँ निकालता है। |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | दस्तावेज़ पृष्ठ से टेबल निकालता है. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | दस्तावेज़ से टेक्स्ट निकालता है. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | दस्तावेज़ पृष्ठ से टेक्स्ट निकालता है. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | पाठ विकल्पों का उपयोग करके दस्तावेज़ से एक पाठ पृष्ठ निकालता है (कच्चे तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)। |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | पाठ विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से एक पाठ निकालता है (कच्चे तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | दस्तावेज़ से पाठ क्षेत्रों को निकालता है। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्र निकालता है. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, मैच केस, आदि) का उपयोग करके दस्तावेज़ से टेक्स्ट क्षेत्र निकालता है। |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, मैच केस, आदि) का उपयोग करके दस्तावेज़ पृष्ठ से पाठ क्षेत्रों को निकालता है। |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | दस्तावेज़ से सामग्री की तालिका निकालता है। |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | उपयोगकर्ता द्वारा उत्पन्न टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है। |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | दस्तावेज़ फ़ॉर्म को पार्स करता है. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | खोजता है*keyword* दस्तावेज़ में. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | खोजता है*keyword*दस्तावेज़ में खोज विकल्प (रेगुलर एक्सप्रेशन, मैच केस, आदि) का उपयोग करके . |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |

### यह सभी देखें

* नाम स्थान [GroupDocs.Parser](../../groupdocs.parser)
* सभा [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
