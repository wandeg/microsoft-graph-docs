---
title: "deviceManagementExchangeAccessState enum type"
description: "Device Exchange Access State."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# deviceManagementExchangeAccessState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device Exchange Access State.

## Members

| Member      | Value | Description                                |
| :---------- | ----: | :----------------------------------------- |
| none        | 0     | No access state discovered from Exchange   |
| unknown     | 1     | Device access state to Exchange is unknown |
| allowed     | 2     | Device has access to Exchange              |
| blocked     | 3     | Device is Blocked in Exchange              |
| quarantined | 4     | Device is Quarantined in Exchange          |