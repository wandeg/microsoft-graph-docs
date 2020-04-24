---
title: "Update target"
description: "Update the properties of a target object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update target

Namespace: microsoft.graph

Update the properties of a target object.

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
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}/target
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
  "name": "update_target"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}/target
Content-Type: application/json
Content-length: 343

{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "objectId": "Object Id value",
  "altSecId": "Alt Sec Id value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "type": "Type value"
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
  "id": "47c5f617-f617-47c5-17f6-c54717f6c547",
  "objectId": "Object Id value",
  "altSecId": "Alt Sec Id value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "type": "Type value"
}
```

