---
title: "Update accessPackageSubject"
description: "Update the properties of an accessPackageSubject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageSubject

Namespace: microsoft.graph

Update the properties of an accessPackageSubject object.

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
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageSubject
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

If successful, this method returns a `200 OK` response code and an updated [accessPackageSubject](../resources/accesspackagesubject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackagesubject"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageSubject
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

