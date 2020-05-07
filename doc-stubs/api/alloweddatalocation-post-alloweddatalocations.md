---
title: "Create allowedDataLocation"
description: "Create a new allowedDataLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create allowedDataLocation

Namespace: microsoft.graph

Create a new [allowedDataLocation](../resources/alloweddatalocation.md) object.

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
POST /allowedDataLocations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [allowedDataLocation](../resources/alloweddatalocation.md) object.

The following table shows the properties that are required when you create the [allowedDataLocation](../resources/alloweddatalocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appId|String|**TODO: Add Description**|
|location|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|domain|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [allowedDataLocation](../resources/alloweddatalocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_alloweddatalocation_from_alloweddatalocations"
}
-->
``` http
POST https://graph.microsoft.com/beta/allowedDataLocations
Content-Type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.allowedDataLocation",
  "appId": "String",
  "location": "String",
  "isDefault": "Boolean",
  "domain": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alloweddatalocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.allowedDataLocation",
  "id": "2c5a6375-6375-2c5a-7563-5a2c75635a2c",
  "appId": "String",
  "location": "String",
  "isDefault": "Boolean",
  "domain": "String"
}
```

