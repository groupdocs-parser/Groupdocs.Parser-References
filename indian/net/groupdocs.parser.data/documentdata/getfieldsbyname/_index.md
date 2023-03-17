---
title: GetFieldsByName
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: फ़ल्ड डेट क संग्रह लटत है जहँ नम इसके बरबर हत हैfieldName .
type: docs
weight: 50
url: /hi/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---
## DocumentData.GetFieldsByName method

फ़ील्ड डेटा का संग्रह लौटाता है जहाँ नाम इसके बराबर होता है*fieldName* .

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldName | String | मैदान का नाम। |

### प्रतिलाभ की मात्रा

का एक संग्रह[`FieldData`](../../fielddata) वस्तुएं; कोई फ़ील्ड डेटा नहीं मिलने पर खाली संग्रह।

### उदाहरण

फ़ील्ड नाम से फ़ील्ड खोजें:

[`FieldData`](../../fielddata) वर्ग फ़ील्ड डेटा का प्रतिनिधित्व करता है। मैदान पर निर्भर करता है[`PageArea`](../../fielddata/pagearea) property में इनमें से कोई भी विरासत हो सकती है[`PageArea`](../../pagearea) कक्षा। उदाहरण के लिए,[`ParseForm`](../../../groupdocs.parser/parser/parseform) method केवल टेक्स्ट फ़ील्ड निकालता है।

```csharp
// "पता" नाम के साथ सभी फ़ील्ड प्राप्त करें
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // खेतों के संग्रह पर पुनरावृति करें
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // यदि यह संबंधित क्षेत्र है:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

### यह सभी देखें

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* नाम स्थान [GroupDocs.Parser.Data](../../documentdata)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->