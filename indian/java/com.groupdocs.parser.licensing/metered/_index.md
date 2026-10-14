---
title: "मापित"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "मीटरड कुंजी सेट करने के लिए मेथड प्रदान करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

मीटरड कुंजी सेट करने के लिए मेथड प्रदान करता है।

इस उदाहरण में, metered सार्वजनिक और निजी कुंजी सेट करने का प्रयास किया जाएगा:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Metered()](#Metered--) | नए उदाहरण को प्रारंभ करता है [Metered](../../com.groupdocs.parser.licensing/metered) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | metered सार्वजनिक और निजी कुंजी सेट करता है। |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | प्रसंस्कृत MBs की मात्रा प्राप्त करता है। |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | उपयोग किए गए क्रेडिट की गिनती प्राप्त करता है। |
|
### Metered() {#Metered--}
```
public Metered()
```


नए उदाहरण को प्रारंभ करता है [Metered](../../com.groupdocs.parser.licensing/metered) क्लास का।


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


metered सार्वजनिक और निजी कुंजी सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | publicKey | java.lang.String | एक सार्वजनिक कुंजी। |
|
|  | privateKey | java.lang.String | एक निजी कुंजी |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


प्रसंस्कृत MBs की मात्रा प्राप्त करता है।


**Returns:**
java.math.BigDecimal - उपभोग मात्रा को दर्शाने वाला एक डबल मान।

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


उपयोग किए गए क्रेडिट की गिनती प्राप्त करता है।


**Returns:**
java.math.BigDecimal - उपभोग क्रेडिट को दर्शाने वाला एक डबल मान।

