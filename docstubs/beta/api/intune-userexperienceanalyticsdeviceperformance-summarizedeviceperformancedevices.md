---
title: "userexperienceanalyticsdeviceperformance : summarizeDevicePerformanceDevices"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# userexperienceanalyticsdeviceperformance : summarizeDevicePerformanceDevices

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

$(this.methodDescription)

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Function parameters

In the request url, provide the following query parameters with values.

The following table shows the parameters that can be used with this method.

| Parameter   | Type   | Description |
| :---------- | :----- | :---------- |
| summarizeBy | String |             |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 Ok` response code.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "userexperienceanalyticsdeviceperformance_summarizedeviceperformancedevices"
}
-->

```http
GET https://graph.microsoft.com/beta/

```

### Response

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "$(this.ReturnTypeFullName)"
}
-->

```http
HTTP 1.1 200 Ok

```