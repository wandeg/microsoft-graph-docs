---
title: "privilegedApproval: myRequests"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# myRequests

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /privilegedApproval/myRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [privilegedApproval](../resources/privilegedapproval.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
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

