---
title: "Get office365ActivationsUserDetail"
description: "Read properties and relationships of the office365ActivationsUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get office365ActivationsUserDetail

Read properties and relationships of the [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object.

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
GET ** Entity URI for microsoft.graph.office365ActivationsUserDetail not found
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
If successful, this method returns a `200 OK` response code and [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_office365activationsuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.office365ActivationsUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": {
    "@odata.type": "#microsoft.graph.office365ActivationsUserDetail",
    "id": "fe7dd89d-d89d-fe7d-9dd8-7dfe9dd87dfe",
    "reportRefreshDate": "Date",
    "userPrincipalName": "User Principal Name value",
    "displayName": "Display Name value",
    "userActivationCounts": [
      {
        "@odata.type": "microsoft.graph.userActivationCounts",
        "productType": "Product Type value",
        "lastActivatedDate": "Date",
        "windows": 7,
        "mac": 3,
        "windows10Mobile": 15,
        "ios": 3,
        "android": 7,
        "activatedOnSharedComputer": true
      }
    ]
  }
}
```

