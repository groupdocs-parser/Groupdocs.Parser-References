---
title: "TemplateTable"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "UPPER CASE 이름으로 TemplateTablegroupdocs.parser.templates/templatetable 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

UPPER CASE 이름으로 [`TemplateTable`](../../templatetable) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| layout | TemplateTableLayout | 테이블 레이아웃. |
| name | 문자열 | 테이블 이름. |

### 예제

테이블을 자동으로 감지할 수 없는 경우 템플릿 테이블은 테이블 레이아웃에 의해 설정됩니다:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// 문서 템플릿 만들기
Template template = new Template(new TemplateItem[] { table });
```

### 참고

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

UPPER CASE 이름으로 [`TemplateTable`](../../templatetable) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| layout | TemplateTableLayout | 테이블 레이아웃. |
| name | 문자열 | 테이블 이름. |
| pageWidth | Nullable`1 | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |

### 예제

테이블을 자동으로 감지할 수 없는 경우 템플릿 테이블은 테이블 레이아웃에 의해 설정됩니다:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// 문서 템플릿 만들기
Template template = new Template(new TemplateItem[] { table });
```

### 참고

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

`[`TemplateTable`](../../templatetable)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| layout | TemplateTableLayout | 테이블 레이아웃. |
| name | 문자열 | 테이블 이름. |
| pageWidth | Nullable`1 | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
| useUpperCaseName | Boolean | `name`이 대문자로 변환되는지 여부를 나타내는 값. |

### 예제

테이블을 자동으로 감지할 수 없는 경우 템플릿 테이블은 테이블 레이아웃에 의해 설정됩니다:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// 문서 템플릿 만들기
Template template = new Template(new TemplateItem[] { table });
```

### 참고

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

`[`TemplateTable`](../../templatetable)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 매개변수 | TemplateTableParameters | 자동 모드에서 표를 감지하기 위한 매개변수입니다. |
| name | 문자열 | 테이블 이름. |

### 예제

감지기 매개변수로 템플릿 표가 설정된 경우, 표가 자동으로 감지됩니다:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// 문서 템플릿 만들기
Template template = new Template(new TemplateItem[] { table });
```

### 참고

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

`[`TemplateTable`](../../templatetable)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 매개변수 | TemplateTableParameters | 자동 모드에서 표를 감지하기 위한 매개변수입니다. |
| name | 문자열 | 테이블 이름. |
| pageWidth | Nullable`1 | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |

### 예제

감지기 매개변수로 템플릿 표가 설정된 경우, 표가 자동으로 감지됩니다:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// 문서 템플릿 만들기
Template template = new Template(new TemplateItem[] { table });
```

### 참고

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

`[`TemplateTable`](../../templatetable)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 매개변수 | TemplateTableParameters | 자동 모드에서 표를 감지하기 위한 매개변수입니다. |
| name | 문자열 | 테이블 이름. |
| pageWidth | Nullable`1 | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
| useUpperCaseName | Boolean | `name`이 대문자로 변환되는지 여부를 나타내는 값. |

### 예제

감지기 매개변수로 템플릿 표가 설정된 경우, 표가 자동으로 감지됩니다:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// 문서 템플릿 만들기
Template template = new Template(new TemplateItem[] { table });
```

### 참고

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
