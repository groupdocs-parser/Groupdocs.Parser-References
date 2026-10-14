---
title: "ParserSettings"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις ρυθμίσεις που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων."
type: docs
weight: 33
url: /el/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Παρέχει τις ρυθμίσεις που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με τον καταγραφέα. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με το OCR Connector. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με το External Resource Handler. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με τον καταγραφέα και το OCR Connector. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getLogger()](#getLogger--) | Λαμβάνει τον καταγραφέα που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων κατά την εξαγωγή δεδομένων. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Λαμβάνει το OCR Connector που χρησιμοποιείται για την παροχή λειτουργικότητας OCR. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Λαμβάνει το χειριστή για εξωτερικούς πόρους. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με τον καταγραφέα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Ένα στιγμιότυπο κλάσης που υλοποιεί τη διεπαφή [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με το OCR Connector.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Ένα στιγμιότυπο κλάσης που κληρονομεί την κλάση [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) για την παροχή λειτουργικότητας OCR. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με το External Resource Handler.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Ένα στιγμιότυπο κλάσης που κληρονομεί την κλάση [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) για την παροχή λειτουργικότητας OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings) με τον καταγραφέα και το OCR Connector.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Ένα στιγμιότυπο κλάσης που υλοποιεί τη διεπαφή [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Ένα στιγμιότυπο κλάσης που κληρονομεί την κλάση [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) για την παροχή λειτουργικότητας OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Ένα στιγμιότυπο κλάσης που υλοποιεί τη διεπαφή [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Ένα στιγμιότυπο κλάσης που κληρονομεί την κλάση [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) για την παροχή λειτουργικότητας OCR. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Ένα στιγμιότυπο κλάσης που κληρονομεί την κλάση [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) για τον έλεγχο της φόρτωσης εξωτερικών πόρων. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Λαμβάνει τον καταγραφέα που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων κατά την εξαγωγή δεδομένων.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Λαμβάνει το OCR Connector που χρησιμοποιείται για την παροχή λειτουργικότητας OCR.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Λαμβάνει το χειριστή για εξωτερικούς πόρους.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

