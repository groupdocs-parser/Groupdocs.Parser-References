---
title: "SetLicense"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Лицензирует компонент."
type: docs
weight: 20
url: /ru/net/groupdocs.parser/license/setlicense/
---

## SetLicense(string) {#setlicense_1}

Лицензирует компонент.

```csharp
public void SetLicense(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Абсолютный путь к файлу лицензии. |

### Примеры

В следующем примере показано, как установить лицензию, передавая путь к файлу лицензии.

```csharp
string licensePath = "LicenseFile.lic"";
GroupDocs.Parser.License license = new GroupDocs.Parser.License();
lic.SetLicense(licensePath);
```

### См. также

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## SetLicense(Stream) {#setlicense}

Лицензирует компонент.

```csharp
public void SetLicense(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток лицензии. |

### Примеры

В следующем примере показано, как установить лицензию, передавая поток файла лицензии.

```csharp
using (FileStream licenseStream = new FileStream("LicenseFile.lic", FileMode.Open))
{
    GroupDocs.Parser.License license = new GroupDocs.Parser.License();
    license.SetLicense(licenseStream);
}
```

### См. также

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
