---
title: Metered class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Manages metered (pay-per-use) licensing."
type: docs
url: /python-net/groupdocs.parser/metered/
is_root: false
weight: 20
---


## Metered class

Manages metered (pay-per-use) licensing.

Metered licenses bill on actual consumption (typically pages or
documents processed). Set the public/private key pair once at
application startup; the wrapper reports usage back to the GroupDocs
license server in the background.

The Metered type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [get_consumption_credit](/parser/python-net/groupdocs.parser/metered/get_consumption_credit/) | Return the number of credits consumed so far. |
| [get_consumption_quantity](/parser/python-net/groupdocs.parser/metered/get_consumption_quantity/) | Return the amount of data processed so far. |
| [set_metered_key](/parser/python-net/groupdocs.parser/metered/set_metered_key/#public_key-private_key) | Activate metered billing with the given public/private key pair. |

### See Also
* module [`groupdocs.parser`](/parser/python-net/groupdocs.parser/)
