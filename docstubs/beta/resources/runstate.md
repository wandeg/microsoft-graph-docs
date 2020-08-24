---
title: "runState enum type"
description: "Indicates the type of execution status of the device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# runState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indicates the type of execution status of the device management script.

## Members

| Member        | Value | Description                               |
| :------------ | ----: | :---------------------------------------- |
| unknown       | 0     | Unknown result.                           |
| success       | 1     | Script is run successfully.               |
| fail          | 2     | Script failed to run.                     |
| scriptError   | 3     | Discovery script hits error.              |
| pending       | 4     | Script is pending to execute.             |
| notApplicable | 5     | Script is not applicable for this device. |