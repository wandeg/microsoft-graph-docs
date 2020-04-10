---
title: "List accessPackageResourceRequests"
description: "List properties and relationships of the accessPackageResourceRequest objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageResourceRequests

Namespace: microsoft.graph

List properties and relationships of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.

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
GET /accessPackageResourceRequests
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageResourceRequests
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresourcerequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
      "id": "5f7f21aa-21aa-5f7f-aa21-7f5faa217f5f",
      "catalogId": "Catalog Id value",
      "executeImmediately": true,
      "isValidationOnly": true,
      "requestType": "Request Type value",
      "requestState": "Request State value",
      "requestStatus": "Request Status value",
      "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
      "justification": "Justification value"
    }
  ]
}
```

