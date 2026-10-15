---
title: "MoveTo"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Erstellt ein neues Layout mit denselben Größen, Trennlinien und Position im Punkt."
type: docs
weight: 50
url: /de/net/groupdocs.parser.templates/templatetablelayout/moveto/
---

## TemplateTableLayout.MoveTo method

Erstellt ein neues Layout mit derselben Größe, denselben Trennzeichen und Position im *Punkt*.

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Punkt | Point | Die Position des neuen Layouts. |

### Rückgabewert

Ein neues Layout mit derselben Größe, den Trennlinien und der Position im *Punkt*.

### Beispiele

Diese Funktionalität ermöglicht das Verschieben von Table Layout.

Beispielsweise enthält ein Dokument auf jeder Seite Tabellen (oder ein Satz von Dokumenten mit einer Tabelle auf der Seite). Diese Tabellen unterscheiden sich in Position und Inhalt, haben jedoch dieselben Spalten und Zeilen. In diesem Fall kann ein Benutzer ein [`TemplateTableLayout`](../../templatetablelayout)-Objekt einmal bei `(0, 0)` definieren und es dann an den Ort der gewünschten Tabelle verschieben.

Wenn die Tabellenposition von einem anderen Objekt der Seite abhängt, kann ein Benutzer ein [`TemplateTableLayout`](../../templatetablelayout)-Objekt basierend auf dem Vorlagendokument definieren und es dann gemäß einem Ankerobjekt verschieben. Beispielsweise, wenn es sich um eine Zusammenfassungstabelle handelt, die von einer Detailtabelle gefolgt wird (die eine unterschiedliche Zeilenanzahl enthalten kann). In diesem Fall kann ein Benutzer ein [`TemplateTableLayout`](../../templatetablelayout)-Objekt im Vorlagendokument (mit dem bekannten Rechteck der Detailtabelle) definieren und dann das [`TemplateTableLayout`](../../templatetablelayout)-Objekt entsprechend der Differenz des Detailtabellen-Rechtecks zwischen Vorlage und realem Dokument verschieben.

`MoveTo`-Methode gibt eine Kopie des aktuellen Objekts zurück. Ein Benutzer kann beliebige Koordinaten übergeben (auch negative – dann wird das Layout nach links/oben verschoben).

```csharp
// Erstelle ein Tabellenlayout
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Drucke ein Rechteck
Rectangle rect = layout.Rectangle;

// Druckt: pos: (0, 0) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Verschiebe das Layout an den genauen Tabellenort
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// Stellen Sie sicher, dass die ersten Trennzeichen verschoben werden:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// Gibt aus: pos: (315, 250) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// Das movedLayout-Objekt ist eine Kopie des layout-Objekts, sodass wir die Trennzeichen anpassen können, ohne das Originallayout zu beeinflussen:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### Siehe auch

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
