---
title: "getOffice365ActivationsUserDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOffice365ActivationsUserDetail

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
GET /reports/getOffice365ActivationsUserDetail
GET /print/reports/{reportRootId}/getOffice365ActivationsUserDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365activationsuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365ActivationsUserDetail",
      "id": "85b3aae9-aae9-85b3-e9aa-b385e9aab385",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "displayName": "Display Name value",
      "userActivationCounts": [
        {
          "@odata.type": "microsoft.graph.userActivationCounts"
        }
      ]
    }
  ]
}
```

