---
title: "License"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "GroupDocs.Parser ライセンスを表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

GroupDocs.Parser ライセンスを表します。

この例では、ライセンスの設定方法を示しています。

````
 ```

// License クラスを初期化
License license = new License();
// .lic ファイルへのパスを設定
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [License()](#License--) | 新しい [License](../../com.groupdocs.parser.licensing/license) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | コンポーネントにライセンスを適用します。 |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | コンポーネントにライセンスを適用します。 |
|
### License() {#License--}
```
public License()
```


新しい [License](../../com.groupdocs.parser.licensing/license) クラスのインスタンスを初期化します。


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


コンポーネントにライセンスを適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ライセンスファイルへの絶対パス。 |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


コンポーネントにライセンスを適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | stream | java.io.InputStream | ライセンスストリーム。 |
|

