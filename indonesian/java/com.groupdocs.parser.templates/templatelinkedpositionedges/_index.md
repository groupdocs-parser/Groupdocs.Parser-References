---
title: "TemplateLinkedPositionEdges"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan tepi bidang yang ditautkan tempat bidang teks dicari."
type: docs
weight: 16
url: /id/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Menyediakan tepi dari bidang yang terhubung tempat bidang teks dicari. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) digunakan dalam kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Menginisialisasi instance baru dari kelas [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Mendapatkan nilai yang menunjukkan apakah instance kosong. |
|
|  | [isLeft()](#isLeft--) | Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari kiri bidang yang terhubung. |
|
|  | [isTop()](#isTop--) | Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari atas bidang yang terhubung. |
|
|  | [isRight()](#isRight--) | Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari kanan bidang yang terhubung. |
|
|  | [isBottom()](#isBottom--) | Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari bawah bidang yang terhubung. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Mengonversi representasi string dari tepi ke ekivalen kelasnya. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Menginisialisasi instance baru dari kelas [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kiri | boolean | Nilai yang menunjukkan apakah sebuah bidang dicari dari kiri bidang yang terhubung. |
|
|  | atas | boolean | Nilai yang menunjukkan apakah sebuah bidang dicari dari atas bidang yang terhubung. |
|
|  | kanan | boolean | Nilai yang menunjukkan apakah sebuah bidang dicari dari kanan bidang yang terhubung. |
|
|  | bawah | boolean | Nilai yang menunjukkan apakah sebuah bidang dicari dari bawah bidang yang terhubung. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Mendapatkan nilai yang menunjukkan apakah instance kosong.


**Returns:**
boolean -  true  jika instance kosong (semua bidang adalah  false ); selain itu,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari kiri bidang yang terhubung.


**Returns:**
boolean -  true  jika sebuah bidang dicari dari kiri bidang yang terhubung; selain itu,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari atas bidang yang terhubung.


**Returns:**
boolean -  true  jika sebuah bidang dicari dari atas bidang yang terhubung; selain itu,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari kanan bidang yang terhubung.


**Returns:**
boolean -  true  jika sebuah bidang dicari dari kanan bidang yang terhubung; selain itu,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Mendapatkan nilai yang menunjukkan apakah sebuah bidang dicari dari bawah bidang yang terhubung.


**Returns:**
boolean -  true  jika sebuah bidang dicari dari bawah bidang yang terhubung; selain itu,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Mengonversi representasi string dari tepi ke ekivalen kelasnya.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | s | java.lang.String | String yang berisi tepi untuk dikonversi. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
