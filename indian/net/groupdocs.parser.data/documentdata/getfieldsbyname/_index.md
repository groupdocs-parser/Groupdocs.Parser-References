---
title: "GetFieldsByName"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "फ़ील्ड डेटा का संग्रह लौटाता है जहाँ नाम fieldName के बराबर है।"
type: docs
weight: 50
url: /hi/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---

## DocumentData.GetFieldsByName method

फ़ील्ड डेटा का संग्रह लौटाता है जहाँ नाम *fieldName* के बराबर हो।

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldName | स्ट्रिंग | फ़ील्ड का नाम। |

### रिटर्न वैल्यू

[`FieldData`](../../fielddata) ऑब्जेक्ट्स का संग्रह; यदि कोई फ़ील्ड डेटा नहीं मिला तो खाली संग्रह।

### Examples

फ़ील्ड नाम द्वारा फ़ील्ड्स खोजें:

```csharp
// "Address" नाम वाले सभी फ़ील्ड्स प्राप्त करें
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // फ़ील्ड्स संग्रह पर इटररेट करें
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // यदि यह संबंधित फ़ील्ड है:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields.

### संबंधित देखें

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
