---
title: "TemplateTable"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 테이블을 제공합니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

템플릿 테이블을 제공합니다.

테이블을 정의하는 방법은 두 가지가 있습니다:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스를 UPPER CASE 이름으로 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스를 UPPER CASE 이름으로 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스를 UPPER CASE 이름으로 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getLayout()](#getLayout--) | 테이블 레이아웃을 가져옵니다. |
|
|  | [getParameters()](#getParameters--) | 자동 모드에서 테이블을 감지하기 위한 매개변수를 가져옵니다. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스를 UPPER CASE 이름으로 새 인스턴스를 초기화합니다.

테이블을 자동으로 감지할 수 없는 경우 테이블 레이아웃에 따라 템플릿 테이블이 설정됩니다:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 테이블 레이아웃. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스를 UPPER CASE 이름으로 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 테이블 레이아웃. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 테이블 레이아웃. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 테이블 레이아웃. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스를 UPPER CASE 이름으로 새 인스턴스를 초기화합니다.

감지기 매개변수로 템플릿 테이블이 설정된 경우, 테이블이 자동으로 감지됩니다:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 자동 모드에서 테이블을 감지하기 위한 매개변수입니다. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 자동 모드에서 테이블을 감지하기 위한 매개변수입니다. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 자동 모드에서 테이블을 감지하기 위한 매개변수입니다. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 자동 모드에서 테이블을 감지하기 위한 매개변수입니다. |
|
|  | 이름 | java.lang.String | 테이블 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 테이블이 위치한 페이지의 인덱스; 템플릿 테이블이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


테이블 레이아웃을 가져옵니다.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


자동 모드에서 테이블을 감지하기 위한 매개변수를 가져옵니다.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


주어진 계수를 사용하여 모든 좌표를 스케일링한 현재 항목의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
