---
title: "Create windowsManagementAppHealthSummary"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create windowsManagementAppHealthSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new windowsManagementAppHealthSummary object.

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

In the request body, supply JSON representation of the windowsManagementAppHealthSummary object.

The following table shows the properties that are required when you create the windowsManagementAppHealthSummary object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthSummary](../resources/windowsManagementAppHealthSummary.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_windowsmanagementapphealthsummary"
}
-->

```http
POST https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 179

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": "Int32",
  "unhealthyDeviceCount": "Int32",
  "unknownDeviceCount": "Int32"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.windowsManagementAppHealthSummary"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": "Int32",
  "id": "String(identifier)",
  "unhealthyDeviceCount": "Int32",
  "unknownDeviceCount": "Int32"
}
}

```