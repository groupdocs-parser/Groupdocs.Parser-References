---
title: "TemplateOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller alternativen som används för parsning via mallfunktionaliteten."
type: docs
weight: 17
url: /sv/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Tillhandahåller alternativen som används för parsning via mallfunktionaliteten.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Initierar en ny instans av klassen [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Hämtar storleken på kanten som ignoreras när den fångas av det rektangulära området. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Initierar en ny instans av klassen [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangleTolerance | double | Storleken på kanten som ignoreras när den fångas av det rektangulära området. Den mäts som en bråkdel av en textrads höjd. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Hämtar storleken på kanten som ignoreras när den fångas av det rektangulära området. Den mäts som en bråkdel av en textrads höjd.


**Returns:**
double - Det dubbla värdet från 0 (ingen kant) till 1 (ignorera hela elementet).

