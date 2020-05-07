---
title: "Add detectedApps"
description: "Add detectedApps by posting to the detectedApps collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add detectedApps

Namespace: microsoft.graph

Add detectedApps by posting to the detectedApps collection.

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
POST /users/{usersId}/managedDevices/{managedDeviceId}/detectedApps/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [detectedApp](../resources/detectedapp.md) object.

The following table shows the properties that are required when you create the [detectedApp](../resources/detectedapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|
|sizeInByte|Int64|**TODO: Add Description**|
|deviceCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [detectedApp](../resources/detectedapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_detectedapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/detectedApps/$ref
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "String",
  "version": "String",
  "sizeInByte": "Integer",
  "deviceCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.detectedapp"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "c6e87af9-7af9-c6e8-f97a-e8c6f97ae8c6",
  "displayName": "String",
  "version": "String",
  "sizeInByte": "Integer",
  "deviceCount": "Integer"
}
```

