---
title: "Get windowsManagementAppHealthState"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get windowsManagementAppHealthState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships a windowsManagementAppHealthState object.

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

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [windowsManagementAppHealthState](../resources/windowsManagementAppHealthState.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_windowsmanagementapphealthstate"
}
-->

```http
GET https://graph.microsoft.com/beta/

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.windowsManagementAppHealthState"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "deviceName": "String",
  "deviceOSVersion": "String",
  "healthState": "String",
  "id": "String(identifier)",
  "installedVersion": "String",
  "lastCheckInDateTime": "DateTimeOffset"
}
}

```