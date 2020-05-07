---
title: "Create requestor"
description: "Create a new requestor object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create requestor

Namespace: microsoft.graph

Create a new requestor object.

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
POST /accessPackageResourceRequests/{accessPackageResourceRequestsId}/requestor
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageSubject](../resources/accesspackagesubject.md) object.

The following table shows the properties that are required when you create the [accessPackageSubject](../resources/accesspackagesubject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|objectId|String|**TODO: Add Description**|
|altSecId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [accessPackageSubject](../resources/accesspackagesubject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackagesubject_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageResourceRequests/{accessPackageResourceRequestsId}/requestor
Content-Type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "objectId": "String",
  "altSecId": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "onPremisesSecurityIdentifier": "String",
  "type": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackagesubject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "af6892e4-92e4-af68-e492-68afe49268af",
  "objectId": "String",
  "altSecId": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "onPremisesSecurityIdentifier": "String",
  "type": "String"
}
```

