---
title: "SetLicense"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "コンポーネントにライセンスを付与します。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser/license/setlicense/
---

## SetLicense(string) {#setlicense_1}

コンポーネントにライセンスを付与します。

```csharp
public void SetLicense(string filePath)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ライセンスファイルへの絶対パス。 |

### 例

次の例は、ライセンスファイルへのパスを渡してライセンスを設定する方法を示します。

```csharp
string licensePath = "LicenseFile.lic"";
GroupDocs.Parser.License license = new GroupDocs.Parser.License();
lic.SetLicense(licensePath);
```

### 関連項目

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## SetLicense(Stream) {#setlicense}

コンポーネントにライセンスを付与します。

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ストリーム | Stream | ライセンスストリーム。 |

### 例

次の例は、ライセンスファイルの Stream を渡してライセンスを設定する方法を示します。

```csharp
using (FileStream licenseStream = new FileStream("LicenseFile.lic", FileMode.Open))
{
    GroupDocs.Parser.License license = new GroupDocs.Parser.License();
    license.SetLicense(licenseStream);
}
```

### 関連項目

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
