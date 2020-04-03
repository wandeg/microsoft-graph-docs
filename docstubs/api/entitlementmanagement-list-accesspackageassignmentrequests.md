---
title: "List accessPackageAssignmentRequests"
description: "Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageAssignmentRequests

Namespace: microsoft.graph

Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property.

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
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "3ccc96a8-96a8-3ccc-a896-cc3ca896cc3c",
      "requestType": "Request Type value",
      "requestState": "Request State value",
      "requestStatus": "Request Status value",
      "isValidationOnly": true,
      "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
      "completedDate": "2017-01-01T00:01:54.8809963+00:00",
      "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
      "justification": "Justification value"
    }
  ]
}
```

