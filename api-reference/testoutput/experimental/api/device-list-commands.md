---
title: "List commands"
description: "Get the commands from the commands navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List commands

Get the commands from the commands navigation property.

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
GET https://graph.microsoft.com/docs\api/devices/{devicesId}/commands
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
      "id": "4b16bcad-bcad-4b16-adbc-164badbc164b",
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

