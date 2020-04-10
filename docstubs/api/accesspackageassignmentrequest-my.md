---
title: "accessPackageAssignmentRequest: My"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# My

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
GET /accessPackageAssignmentRequests/My
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/My
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests/My
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests/My
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignmentRequests/My
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
      "id": "0c229a9b-9a9b-0c22-9b9a-220c9b9a220c",
      "requestType": "Request Type value",
      "requestState": "Request State value",
      "requestStatus": "Request Status value",
      "isValidationOnly": true,
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "completedDate": "2016-12-31T23:57:54.3086791+00:00",
      "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
      "justification": "Justification value"
    }
  ]
}
```

