---
title: "actionState enum type"
description: "State of the action on the device"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# actionState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

State of the action on the device

## Members

| Member       | Value | Description                      |
| :----------- | ----: | :------------------------------- |
| none         | 0     | Not a valid action state         |
| pending      | 1     | Action is pending                |
| canceled     | 2     | Action has been cancelled.       |
| active       | 3     | Action is active.                |
| done         | 4     | Action completed without errors. |
| failed       | 5     | Action failed                    |
| notSupported | 6     | Action is not supported.         |