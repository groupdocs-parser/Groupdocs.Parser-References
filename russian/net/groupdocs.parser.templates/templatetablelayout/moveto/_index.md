---
title: MoveTo
second_title: Справочник по API GroupDocs.Parser для .NET
description: Создает новый макет с тем же размером разделителями и положением вpoint .
type: docs
weight: 50
url: /ru/net/groupdocs.parser.templates/templatetablelayout/moveto/
---
## TemplateTableLayout.MoveTo method

Создает новый макет с тем же размером, разделителями и положением в*point* .

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| point | Point | Положение нового макета. |

### Возвращаемое значение

Новый макет с тем же размером, разделителями и положением в*point*.

### Примеры

Эта функция позволяет перемещать макет таблицы.

Например, в документе есть таблицы на каждой странице (или набор документов с таблицей на странице). Эти таблицы различаются по положению и содержимому, но имеют одни и те же столбцы и строки. В этом случае пользователь может определить [`TemplateTableLayout`](../../templatetablelayout) объект в`(0, 0)` один раз, а затем переместите его на место определенной таблицы.

Если позиция таблицы зависит от другого объекта страницы, пользователь может определить[`TemplateTableLayout`](../../templatetablelayout) объект на основе на шаблоне документа, а затем переместите его в соответствии с объектом привязки. Например, если это сводная таблица и , за ней следует подробная таблица (которая может содержать другое количество строк). В этом случае пользователь может определить [`TemplateTableLayout`](../../templatetablelayout)объект в шаблоне документа (с прямоугольником таблицы известных сведений), а затем переместите [`TemplateTableLayout`](../../templatetablelayout) объект в соответствии с разницей прямоугольника таблицы деталей шаблона и реального документа.

`MoveTo` метод возвращает копию текущего объекта. Пользователь может передавать любые координаты (даже отрицательные - тогда макет будет перемещен влево/вверх).

```csharp
// Создаем макет таблицы
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Печать прямоугольника
Rectangle rect = layout.Rectangle;

// Выводит: pos: (0, 0) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Переместить макет в определенное место таблицы
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// Убедитесь, что первые разделители перемещены:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // печатает: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // печатает: 250

Rectangle movedRect = movedLayout.Rectangle;

// Печатает: pos: (315, 250) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// Объект moveLayout является копией объекта макета, поэтому мы можем настроить разделители без влияния на исходный макет:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // печатает: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // печатает: 6
```

### Смотрите также

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* пространство имен [GroupDocs.Parser.Templates](../../templatetablelayout)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
