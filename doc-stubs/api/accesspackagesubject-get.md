---
title: "Get accessPackageSubject"
description: "Read the properties and relationships of an accessPackageSubject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get accessPackageSubject

Namespace: microsoft.graph

Read the properties and relationships of an [accessPackageSubject](../resources/accesspackagesubject.md) object.

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
GET /accessPackageAssignments/{accessPackageAssignmentsId}/target
GET /accessPackageResourceRequests/{accessPackageResourceRequestsId}/requestor
GET /accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}/requestor
GET /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageSubject
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [accessPackageSubject](../resources/accesspackagesubject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackagesubject"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}/target
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageSubject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

