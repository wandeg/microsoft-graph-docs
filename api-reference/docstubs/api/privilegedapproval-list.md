---
title: "List privilegedApprovals"
description: "Get a list of the privilegedApproval objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List privilegedApprovals

Namespace: microsoft.graph

Get a list of the [privilegedApproval](../resources/privilegedapproval.md) objects and their properties.

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
GET /privilegedApproval
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
If successful, this method returns a `200 OK` response code and a collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedApproval
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedapproval)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedApproval",
      "id": "fe571cdc-1cdc-fe57-dc1c-57fedc1c57fe",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "approvalType": "Approval Type value",
      "approvalState": "String",
      "approvalDuration": "-PT1M43.8104246S",
      "requestorReason": "Requestor Reason value",
      "approverReason": "Approver Reason value",
      "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
      "endDateTime": "2016-12-31T23:59:06.8319712+03:00"
    }
  ]
}
```

