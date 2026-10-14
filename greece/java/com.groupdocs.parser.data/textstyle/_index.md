---
title: "TextStyle"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει το στυλ του κειμένου, όπως το όνομα γραμματοσειράς, το μέγεθος γραμματοσειράς κ.λπ."
type: docs
weight: 30
url: /el/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Αντιπροσωπεύει το στυλ του κειμένου όπως όνομα γραμματοσειράς, μέγεθος γραμματοσειράς κ.λπ.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getName()](#getName--) | Αποκτά το όνομα του στυλ. |
|
|  | [getFontName()](#getFontName--) | Αποκτά το όνομα της γραμματοσειράς. |
|
|  | [getFontSize()](#getFontSize--) | Λαμβάνει το μέγεθος της γραμματοσειράς. |
|
|  | [isBold()](#isBold--) | Λαμβάνει την τιμή που υποδεικνύει αν η γραμματοσειρά είναι έντονη. |
|
|  | [isItalic()](#isItalic--) | Λαμβάνει την τιμή που υποδεικνύει αν η γραμματοσειρά είναι πλάγια. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | όνομα | java.lang.String | Το όνομα του στυλ. |
|
|  | fontName | java.lang.String | Το όνομα της γραμματοσειράς. |
|
|  | fontSize | double | Το μέγεθος της γραμματοσειράς. |
|
|  | bold | boolean | Η τιμή που υποδεικνύει αν η γραμματοσειρά είναι έντονη. |
|
|  | italic | boolean | Η τιμή που υποδεικνύει αν η γραμματοσειρά είναι πλάγια. |
|

### getName() {#getName--}
```
public String getName()
```


Αποκτά το όνομα του στυλ.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το όνομα του στυλ.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Αποκτά το όνομα της γραμματοσειράς.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το όνομα της γραμματοσειράς.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Λαμβάνει το μέγεθος της γραμματοσειράς.


**Returns:**
double - Μια τιμή τύπου double που αντιπροσωπεύει το μέγεθος της γραμματοσειράς.

### isBold() {#isBold--}
```
public boolean isBold()
```


Λαμβάνει την τιμή που υποδεικνύει αν η γραμματοσειρά είναι έντονη.


**Returns:**
boolean -  true  αν η γραμματοσειρά είναι έντονη; διαφορετικά,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Λαμβάνει την τιμή που υποδεικνύει αν η γραμματοσειρά είναι πλάγια.


**Returns:**
boolean -  true  αν η γραμματοσειρά είναι πλάγια; διαφορετικά,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
