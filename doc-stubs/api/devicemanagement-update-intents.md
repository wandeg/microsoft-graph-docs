---
title: "Update intents"
description: "Update the properties of an intents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update intents

Namespace: microsoft.graph

Update the properties of an intents object.

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
PATCH /deviceManagement/intents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementIntent](../resources/devicemanagementintent.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/devicemanagementintent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|isAssigned|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/devicemanagementintent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_intents"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents
Content-Type: application/json
Content-length: 219

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "String",
  "description": "String",
  "isAssigned": "Boolean",
  "templateId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "fc6ac71c-c71c-fc6a-1cc7-6afc1cc76afc",
  "displayName": "String",
  "description": "String",
  "isAssigned": "Boolean",
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

