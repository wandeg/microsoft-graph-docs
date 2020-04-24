---
title: "Update operations"
description: "Update the properties of an operations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update operations

Namespace: microsoft.graph

Update the properties of an operations object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [onenoteOperation](../resources/onenoteoperation.md) object.

The following table shows the properties that are required when you create the [onenoteOperation](../resources/onenoteoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|operationStatus|**TODO: Add Description** Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [operation](../resources/operation.md)|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [operation](../resources/operation.md)|
|resourceLocation|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|error|[onenoteOperationError](../resources/onenoteoperationerror.md)|**TODO: Add Description**|
|percentComplete|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [onenoteOperation](../resources/onenoteoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_operations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
Content-Type: application/json
Content-length: 419

{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:57:13.8078619+03:00",
  "resourceLocation": "Resource Location value",
  "resourceId": "Resource Id value",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError",
    "code": "Code value",
    "message": "Message value"
  },
  "percentComplete": "Percent Complete value"
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
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "2291d582-d582-2291-82d5-912282d59122",
  "status": "String",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastActionDateTime": "2016-12-31T23:57:13.8078619+03:00",
  "resourceLocation": "Resource Location value",
  "resourceId": "Resource Id value",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError",
    "code": "Code value",
    "message": "Message value"
  },
  "percentComplete": "Percent Complete value"
}
```

