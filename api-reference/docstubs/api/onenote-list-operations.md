---
title: "List operations"
description: "Get the onenoteOperations from the operations navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

Get the onenoteOperations from the operations navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onenoteOperation](../resources/onenoteoperation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onenoteoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

