---
title: "Update accessPackageResourceRequests"
description: "Update the properties of an accessPackageResourceRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageResourceRequests

Namespace: microsoft.graph

Update the properties of an accessPackageResourceRequests object.

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
PATCH ** Collection URI for microsoft.graph.accessPackageResourceRequest not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|catalogId|String|**TODO: Add Description**|
|executeImmediately|Boolean|**TODO: Add Description**|
|isValidationOnly|Boolean|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|
|requestState|String|**TODO: Add Description**|
|requestStatus|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresourcerequests"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.accessPackageResourceRequest not found
Content-Type: application/json
Content-length: 330

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "catalogId": "String",
  "executeImmediately": "Boolean",
  "isValidationOnly": "Boolean",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "expirationDateTime": "String (timestamp)",
  "justification": "String"
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
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "id": "435d80e8-80e8-435d-e880-5d43e8805d43",
  "catalogId": "String",
  "executeImmediately": "Boolean",
  "isValidationOnly": "Boolean",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "expirationDateTime": "String (timestamp)",
  "justification": "String"
}
```

