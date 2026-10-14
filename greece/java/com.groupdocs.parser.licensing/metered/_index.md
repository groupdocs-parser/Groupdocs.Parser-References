---
title: "Metered"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει μεθόδους για τον ορισμό κλειδιού χρέωσης με μέτρηση."
type: docs
weight: 11
url: /el/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Παρέχει μεθόδους για τον ορισμό κλειδιού χρέωσης με μέτρηση.

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να οριστεί το δημόσιο και το ιδιωτικό κλειδί του metered:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Metered()](#Metered--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Ορίζει το δημόσιο και το ιδιωτικό κλειδί του metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Ανακτά το ποσό των επεξεργασμένων MB. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Ανακτά τον αριθμό των καταναλωμένων πίστωσεων. |
|
### Metered() {#Metered--}
```
public Metered()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Ορίζει το δημόσιο και το ιδιωτικό κλειδί του metered.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | publicKey | java.lang.String | Ένα δημόσιο κλειδί. |
|
|  | privateKey | java.lang.String | Ένα ιδιωτικό κλειδί |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Ανακτά το ποσό των επεξεργασμένων MB.


**Returns:**
java.math.BigDecimal - Μια τιμή double που αντιπροσωπεύει την ποσότητα κατανάλωσης.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Ανακτά τον αριθμό των καταναλωμένων πίστωσεων.


**Returns:**
java.math.BigDecimal - Μια τιμή double που αντιπροσωπεύει την πίστωση κατανάλωσης.

