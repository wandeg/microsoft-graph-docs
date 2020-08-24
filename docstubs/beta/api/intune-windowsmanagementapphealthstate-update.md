---
title: "Update windowsManagementAppHealthState"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update windowsManagementAppHealthState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a windowsManagementAppHealthState object.

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

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the windowsManagementAppHealthState object.

The following table shows the properties that are required when you create the windowsManagementAppHealthState object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [windowsManagementAppHealthState](../resources/windowsManagementAppHealthState.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_windowsmanagementapphealthstate"
}
-->

```http
PATCH https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "deviceName": "String",
  "deviceOSVersion": "String",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "DateTimeOffset"
}

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