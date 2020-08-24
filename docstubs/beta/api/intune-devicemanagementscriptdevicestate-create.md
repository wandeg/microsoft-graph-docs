---
title: "Create deviceManagementScriptDeviceState"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create deviceManagementScriptDeviceState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new deviceManagementScriptDeviceState object.

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

In the request body, supply JSON representation of the deviceManagementScriptDeviceState object.

The following table shows the properties that are required when you create the deviceManagementScriptDeviceState object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/deviceManagementScriptDeviceState.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_devicemanagementscriptdevicestate"
}
-->

```http
POST https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 236

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "errorCode": "Int32",
  "errorDescription": "String",
  "lastStateUpdateDateTime": "DateTimeOffset",
  "resultMessage": "String",
  "runState": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.deviceManagementScriptDeviceState"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "errorCode": "Int32",
  "errorDescription": "String",
  "id": "String(identifier)",
  "lastStateUpdateDateTime": "DateTimeOffset",
  "resultMessage": "String",
  "runState": "String"
}
}

```