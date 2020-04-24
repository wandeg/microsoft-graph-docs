---
title: "accessPackageAssignmentRequest: My"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# My

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
GET /accessPackageAssignmentRequests/My
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/My
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
      "id": "a571c5ac-c5ac-a571-acc5-71a5acc571a5",
      "requestType": "Request Type value",
      "requestState": "Request State value",
      "requestStatus": "Request Status value",
      "isValidationOnly": true,
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "completedDate": "2016-12-31T23:59:42.8740055+03:00",
      "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
      "justification": "Justification value"
    }
  ]
}
```

