---
title: "TextReader"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente un lecteur capable de lire une série séquentielle de caractères."
type: docs
weight: 29
url: /fr/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Représente un lecteur capable de lire une série séquentielle de caractères.

## Constructors

| Constructor | Description |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Methods

| Method | Description |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Lit une ligne de caractères depuis le lecteur de texte et renvoie les données sous forme de chaîne. |
|
|  | [readToEnd()](#readToEnd--) | Lit tous les caractères depuis la position actuelle jusqu'à la fin du lecteur de texte et les renvoie sous forme d'une seule chaîne. |
|
|  | [dispose()](#dispose--) | Libère toutes les ressources utilisées par l'objet [TextReader](../../com.groupdocs.parser.data/textreader). |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


Lit une ligne de caractères depuis le lecteur de texte et renvoie les données sous forme de chaîne.


**Returns:**
java.lang.String - La ligne suivante du lecteur, ou  null  si tous les caractères ont été lus.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Lit tous les caractères depuis la position actuelle jusqu'à la fin du lecteur de texte et les renvoie sous forme d'une seule chaîne.


**Returns:**
java.lang.String - Une chaîne qui contient tous les caractères depuis la position actuelle jusqu'à la fin du lecteur de texte.

### dispose() {#dispose--}
```
public void dispose()
```


Libère toutes les ressources utilisées par l'objet [TextReader](../../com.groupdocs.parser.data/textreader).


