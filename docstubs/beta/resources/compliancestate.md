---
title: "complianceState enum type"
description: "Compliance state."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# complianceState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Compliance state.

## Members

| Member        | Value | Description                                                         |
| :------------ | ----: | :------------------------------------------------------------------ |
| unknown       | 0     | Unknown.                                                            |
| compliant     | 1     | Compliant.                                                          |
| noncompliant  | 2     | Device is non-compliant and is blocked from corporate resources.    |
| conflict      | 3     | Conflict with other rules.                                          |
| error         | 4     | Error.                                                              |
| inGracePeriod | 254   | Device is non-compliant but still has access to corporate resources |
| configManager | 255   | Managed by Config Manager                                           |