---
title: "Get command"
description: "Read properties and relationships of the command object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get command

Namespace: microsoft.graph

Read properties and relationships of the [command](../resources/command.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /commands/{commandsId}
GET /devices/{devicesId}/commands/{commandId}
GET /me/devices/{deviceId}/commands/{commandId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [command](../resources/command.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_command"
}
-->
``` http
GET https://graph.microsoft.com/localtest/commands/{commandsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.command"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 488

{
  "value": {
    "@odata.type": "#microsoft.graph.command",
    "id": "b0b6c364-c364-b0b6-64c3-b6b064c3b6b0",
    "Status": "Status value",
    "Type": "Type value",
    "AppServiceName": "App Service Name value",
    "PackageFamilyName": "Package Family Name value",
    "Error": "Error value",
    "Payload": {
      "@odata.type": "microsoft.graph.PayloadRequest"
    },
    "PermissionTicket": "Permission Ticket value",
    "PostBackUri": "Post Back Uri value"
  }
}
```

