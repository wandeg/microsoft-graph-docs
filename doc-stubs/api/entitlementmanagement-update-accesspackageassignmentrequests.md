---
title: "Update accessPackageAssignmentRequests"
description: "Update the properties of an accessPackageAssignmentRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageAssignmentRequests

Namespace: microsoft.graph

Update the properties of an accessPackageAssignmentRequests object.

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
PATCH ** Collection URI for microsoft.graph.accessPackageAssignmentRequest not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|requestType|String|**TODO: Add Description**|
|requestState|String|**TODO: Add Description**|
|requestStatus|String|**TODO: Add Description**|
|isValidationOnly|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|completedDate|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentrequests"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.accessPackageAssignmentRequest not found
Content-Type: application/json
Content-length: 312

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "isValidationOnly": "Boolean",
  "completedDate": "String (timestamp)",
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
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "1b844ca8-4ca8-1b84-a84c-841ba84c841b",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "isValidationOnly": "Boolean",
  "createdDateTime": "String (timestamp)",
  "completedDate": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "justification": "String"
}
```

