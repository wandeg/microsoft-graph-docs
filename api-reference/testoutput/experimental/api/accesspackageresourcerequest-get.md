---
title: "Get accessPackageResourceRequest"
description: "Read properties and relationships of the accessPackageResourceRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackageResourceRequest

Namespace: microsoft.graph

Read properties and relationships of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /accessPackageResourceRequests/{accessPackageResourceRequestsId}
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests/{accessPackageResourceRequestId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageResourceRequests/{accessPackageResourceRequestsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
    "id": "9d1eccee-ccee-9d1e-eecc-1e9deecc1e9d",
    "catalogId": "Catalog Id value",
    "executeImmediately": true,
    "isValidationOnly": true,
    "requestType": "Request Type value",
    "requestState": "Request State value",
    "requestStatus": "Request Status value",
    "justification": "Justification value",
    "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00"
  }
}
```

