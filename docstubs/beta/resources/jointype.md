---
title: "joinType enum type"
description: "Device enrollment join type."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# joinType enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device enrollment join type.

## Members

| Member              | Value | Description                              |
| :------------------ | ----: | :--------------------------------------- |
| unknown             | 0     | Unknown enrollment join type.            |
| azureADJoined       | 1     | The device is joined by Azure AD.        |
| azureADRegistered   | 2     | The device is registered by Azure AD.    |
| hybridAzureADJoined | 3     | The device is joined by hybrid Azure AD. |