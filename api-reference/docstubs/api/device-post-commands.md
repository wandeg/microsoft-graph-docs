---
title: "Create commands"
description: "Create a new commands object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create commands

Namespace: microsoft.graph

Create a new commands object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /devices/{devicesId}/commands
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [command](../resources/command.md) object.

The following table shows the properties that are required when you create the [command](../resources/command.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|Status|String|**TODO: Add Description**|
|Type|String|**TODO: Add Description**|
|AppServiceName|String|**TODO: Add Description**|
|PackageFamilyName|String|**TODO: Add Description**|
|Error|String|**TODO: Add Description**|
|Payload|[PayloadRequest](../resources/payloadrequest.md)|**TODO: Add Description**|
|PermissionTicket|String|**TODO: Add Description**|
|PostBackUri|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [command](../resources/command.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_command_from_commands"
}
-->
``` http
POST https://graph.microsoft.com/beta/devices/{devicesId}/commands
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.command"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.command",
  "id": "260bf681-f681-260b-81f6-0b2681f60b26",
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

