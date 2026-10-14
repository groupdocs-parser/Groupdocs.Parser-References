---
title: "HighlightOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour extraire un surlignage d'un bloc de texte autour du texte trouvé dans les scénarios de recherche."
type: docs
weight: 22
url: /fr/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Fournit les options utilisées pour extraire une mise en évidence (un bloc de texte autour du texte trouvé dans les scénarios de recherche).

Une instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) est utilisée comme paramètre dans la méthode [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
Voir les exemples d'utilisation là-bas.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sans limites définies. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) qui est utilisée pour extraire un surlignage de longueur fixe. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) qui est utilisée pour extraire un surlignage limité à une ligne. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) qui est utilisée pour extraire un surlignage avec un nombre de mots fixe. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Obtient une longueur maximale du texte. |
|
|  | [getWordCount()](#getWordCount--) | Obtient un nombre maximal de mots. |
|
|  | [isLineLimited()](#isLineLimited--) | Obtient la valeur qui indique si l'extraction du surlignage est limitée par le début (ou la fin) d'une ligne de texte. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Définit une longueur maximale du texte. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Définit un nombre maximal de mots. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Définit la valeur qui indique si l'extraction de surlignage est limitée par le début (ou la fin) d'une ligne de texte. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sans limites définies. Définissez au moins l'une des méthodes #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) avant de la transmettre au parseur.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) qui est utilisée pour extraire un surlignage de longueur fixe.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | maxLength | int | La longueur maximale du texte. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) qui est utilisée pour extraire un surlignage limité à une ligne.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La longueur maximale du texte. |
|
|  | isLineLimited | boolean | La valeur qui indique si l'extraction de surlignage est limitée par le début (ou la fin) d'une ligne de texte. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) qui est utilisée pour extraire un surlignage avec un nombre de mots fixe.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La longueur maximale du texte. |
|
|  | wordCount | int | Le nombre maximal de mots. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Initialise une nouvelle instance de la classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La longueur maximale du texte. |
|
|  | wordCount | java.lang.Integer | Le nombre maximal de mots. |
|
|  | isLineLimited | boolean | La valeur qui indique si l'extraction de surlignage est limitée par le début (ou la fin) d'une ligne de texte. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Obtient une longueur maximale du texte.


**Returns:**
java.lang.Integer - Une valeur entière positive qui représente la longueur maximale du texte ;  null  si la longueur du texte n'est pas limitée.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Obtient un nombre maximal de mots.


**Returns:**
java.lang.Integer - Une valeur entière positive qui représente le nombre maximal de mots ;  null  si le nombre de mots n'est pas limité.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Obtient la valeur qui indique si l'extraction du surlignage est limitée par le début (ou la fin) d'une ligne de texte.


**Returns:**
boolean -  true  si l'extraction de surlignage est limitée par le début (ou la fin) d'une ligne de texte ; sinon,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Définit une longueur maximale du texte.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Un entier non négatif ;  null  pour supprimer la limite de longueur. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Définit un nombre maximal de mots.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Un entier non négatif ;  null  pour supprimer la limite du nombre de mots. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Définit la valeur qui indique si l'extraction de surlignage est limitée par le début (ou la fin) d'une ligne de texte.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | lineLimited | boolean | true  pour limiter aux limites de ligne. |
|

