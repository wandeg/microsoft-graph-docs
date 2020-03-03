---
title: "Add commands"
description: "Add commands by posting to the commands collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add commands

Add commands by posting to the commands collection.

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
POST /devices/{devicesId}/commands/$ref
POST /me/devices/{deviceId}/commands/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the command object.

The following table shows the properties that are required when you create the command.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|Status|String||
|Type|String||
|AppServiceName|String||
|PackageFamilyName|String||
|Error|String||
|Payload|[PayloadRequest](../resources/PayloadRequest.md)||
|PermissionTicket|String||
|PostBackUri|String||



## Response
If successful, this method returns a `201 Created` response code and a [command](../resources/command.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_command_from_commands"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/devices/{devicesId}/commands
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.command",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

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
```

