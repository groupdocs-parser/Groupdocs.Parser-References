---
title: "MoveTo"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Создаёт новый макет с тем же размером, теми же разделителями и позицией в точке."
type: docs
weight: 50
url: /ru/net/groupdocs.parser.templates/templatetablelayout/moveto/
---

## TemplateTableLayout.MoveTo method

Создаёт новый макет с тем же размером, разделителями и позицией в *точке*.

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| point | Point | Позиция нового макета. |

### Возвращаемое значение

Новый макет с тем же размером, разделителями и позицией в *point*.

### Примеры

Эта функция позволяет перемещать макет таблицы.

Например, документ содержит таблицы на каждой странице (или набор документов с таблицей на странице). Эти таблицы различаются позицией и содержимым, но имеют одинаковые столбцы и строки. В этом случае пользователь может определить объект [`TemplateTableLayout`](../../templatetablelayout) в точке `(0, 0)` один раз, а затем переместить его в расположение конкретной таблицы.

Если позиция таблицы зависит от другого объекта на странице, пользователь может определить объект [`TemplateTableLayout`](../../templatetablelayout) на основе шаблонного документа и затем переместить его в соответствии с опорным объектом. Например, если это сводная таблица, за которой следует детальная таблица (которая может содержать различное количество строк). В этом случае пользователь может определить объект [`TemplateTableLayout`](../../templatetablelayout) в шаблонном документе (с известным прямоугольником детальной таблицы) и затем переместить объект [`TemplateTableLayout`](../../templatetablelayout) в соответствии с разницей прямоугольников детальной таблицы шаблона и реального документа.

`MoveTo` метод возвращает копию текущего объекта. Пользователь может передать любые координаты (даже отрицательные — тогда макет будет перемещён влево/вверх).

```csharp
// Создать макет таблицы
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Вывести прямоугольник
Rectangle rect = layout.Rectangle;

// Вывод: pos: (0, 0) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Переместить макет в конкретное расположение таблицы
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// Убедитесь, что первые разделители перемещены:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// Вывод: pos: (315, 250) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// Объект movedLayout является копией объекта layout, поэтому мы можем настраивать разделители без влияния на оригинальный макет:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### См. также

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
