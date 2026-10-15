---
title: "MoveTo"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Crée une nouvelle mise en page avec les mêmes séparateurs de taille et la même position dans le point."
type: docs
weight: 50
url: /fr/net/groupdocs.parser.templates/templatetablelayout/moveto/
---

## TemplateTableLayout.MoveTo method

Crée une nouvelle mise en page avec la même taille, les mêmes séparateurs et la même position dans le *point*.

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| point | Point | La position de la nouvelle mise en page. |

### Valeur de retour

Une nouvelle mise en page avec la même taille, les séparateurs et la position dans le *point*.

### Exemples

Cette fonctionnalité permet de déplacer le Table Layout.

Par exemple, un document possède des tableaux sur chaque page (ou un ensemble de documents avec un tableau sur la page). Ces tableaux diffèrent par leur position et leur contenu, mais ont les mêmes colonnes et lignes. Dans ce cas, un utilisateur peut définir l'objet [`TemplateTableLayout`](../../templatetablelayout) à `(0, 0)` une fois, puis le déplacer vers l'emplacement du tableau définitif.

Si la position du tableau dépend d'un autre objet de la page, un utilisateur peut définir l'objet [`TemplateTableLayout`](../../templatetablelayout) basé sur le document modèle, puis le déplacer selon un objet d'ancrage. Par exemple, s'il s'agit d'un tableau récapitulatif suivi d'un tableau de détails (qui peut contenir un nombre différent de lignes). Dans ce cas, un utilisateur peut définir l'objet [`TemplateTableLayout`](../../templatetablelayout) sur le document modèle (avec le rectangle du tableau de détails connu) puis déplacer l'objet [`TemplateTableLayout`](../../templatetablelayout) selon la différence entre le rectangle du tableau de détails du modèle et du document réel.

La méthode `MoveTo` renvoie une copie de l'objet actuel. Un utilisateur peut fournir n'importe quelles coordonnées (même négatives - alors la disposition sera déplacée vers la gauche/haut).

```csharp
// Créer une disposition de tableau
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Imprimer un rectangle
Rectangle rect = layout.Rectangle;

// Affiche : pos : (0, 0) taille : (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Déplacer la disposition vers l'emplacement du tableau définitif
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// Assurez‑vous que les premiers séparateurs sont déplacés :
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// Affiche : pos : (315, 250) taille : (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// L'objet movedLayout est une copie de l'objet layout, ainsi nous pouvons ajuster les séparateurs sans impacter la disposition originale :
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### Voir aussi

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
