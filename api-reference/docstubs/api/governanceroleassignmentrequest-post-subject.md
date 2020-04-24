---
title: "Create subject"
description: "Create a new subject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create subject

Namespace: microsoft.graph

Create a new subject object.

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
POST /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/subject
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [governanceSubject](../resources/governancesubject.md) object.

The following table shows the properties that are required when you create the [governanceSubject](../resources/governancesubject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|type|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [governanceSubject](../resources/governancesubject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governancesubject_from_governancesubjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/subject
Content-Type: application/json
Content-length: 195

{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "type": "Type value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governancesubject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "id": "2a86869c-869c-2a86-9c86-862a9c86862a",
  "type": "Type value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value"
}
```

