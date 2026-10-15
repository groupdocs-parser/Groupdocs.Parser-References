---
title: "SetMeteredKey"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Активирует продукт с ключами Metered."
type: docs
weight: 20
url: /ru/net/groupdocs.parser/metered/setmeteredkey/
---

## Metered.SetMeteredKey method

Активирует продукт с ключами Metered.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | Строка | Публичный ключ. |
| privateKey | Строка | Приватный ключ |

### Примеры

Следующий пример демонстрирует, как активировать продукт с помощью Metered keys.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### См. также

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
