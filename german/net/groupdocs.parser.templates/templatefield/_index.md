---
title: "TemplateField"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt das Textfeld der Vorlage bereit."
type: docs
weight: 80
url: /de/net/groupdocs.parser.templates/templatefield/
---

## TemplateField class

Stellt das Textfeld der Vorlage bereit.

```csharp
public sealed class TemplateField : TemplateItem
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | Initialisiert eine neue Instanz der [`TemplateField`](../templatefield)-Klasse. |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, double?) | Initialisiert eine neue Instanz der [`TemplateField`](../templatefield)-Klasse. |
| [TemplateField](templatefield#constructor_2)(TemplatePosition, string, double?, bool) | Initialisiert eine neue Instanz der [`TemplateField`](../templatefield)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsHidden](../../groupdocs.parser.templates/templatefield/ishidden) { get; set; } | Liest oder setzt das Flag für ein verstecktes Vorlagenfeld. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Liefert den Namen des Vorlagen-Elements. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Liefert die Breite der Seite, die zum Erstellen des Vorlagen-Elements verwendet wurde. |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | Gibt den Wert zurück, der beschreibt, wie das Vorlagenfeld auf der Dokumentenseite gefunden wird. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Liefert einen booleschen Wert, der angibt, ob ein `Name` in GROSSBUCHSTABEN umgewandelt wurde. |
| [Value](../../groupdocs.parser.templates/templatefield/value) { get; set; } | Liest oder setzt den Wert des Vorlagenfeldes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatefield/scale)(double) | Skaliert dieses Vorlagen-Elements um einen angegebenen Faktor. |

### Hinweise

Textfelder werden durch ihre Position auf der Seite definiert. Es gibt drei Möglichkeiten, ein Textfeld zu definieren:

* [`Using the rectangular area`](../templatefixedposition)
* [`Using the regular expression`](../templateregexposition)
* [`Using the linked field`](../templatelinkedposition)

### Siehe auch

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
