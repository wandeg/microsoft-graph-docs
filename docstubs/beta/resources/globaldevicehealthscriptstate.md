---
title: "globalDeviceHealthScriptState enum type"
description: "Indicates whether global device health scripts are enabled and are in which state"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# globalDeviceHealthScriptState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indicates whether global device health scripts are enabled and are in which state

## Members

| Member        | Value | Description                                                       |
| :------------ | ----: | :---------------------------------------------------------------- |
| notConfigured | 0     | Global device health scripts are not configured                   |
| pending       | 1     | Global device health scripts are configured but not fully enabled |
| enabled       | 2     | Global device health scripts are enabled and ready to use         |