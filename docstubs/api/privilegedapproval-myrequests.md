---
title: "myRequests"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# myRequests

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [privilegedApproval](../resources/privilegedapproval.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedapproval)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedApproval",
      "id": "0b40068f-068f-0b40-8f06-400b8f06400b",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "approvalType": "Approval Type value",
      "approvalState": "String",
      "approvalDuration": "-PT2M41.8674968S",
      "requestorReason": "Requestor Reason value",
      "approverReason": "Approver Reason value",
      "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
      "endDateTime": "2017-01-01T00:01:31.3007329+03:00"
    }
  ]
}
```

