---
title: "List commands"
description: "List properties and relationships of the command objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List commands

Namespace: microsoft.graph

List properties and relationships of the [command](../resources/command.md) objects.

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
GET /commands
GET /devices/{devicesId}/commands
GET /me/devices/{deviceId}/commands
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [command](../resources/command.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_command"
}
-->
``` http
GET https://graph.microsoft.com/localtest/commands
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.command)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": [
    {
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
  ]
}
```

