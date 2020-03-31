---
title: "getCredentialUserRegistrationCount"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getCredentialUserRegistrationCount

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
GET /reports/getCredentialUserRegistrationCount
GET /print/reports/{reportRootId}/getCredentialUserRegistrationCount
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.credentialuserregistrationcount)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
      "id": "eacbe3b9-e3b9-eacb-b9e3-cbeab9e3cbea",
      "totalUserCount": 14,
      "userRegistrationCounts": [
        {
          "@odata.type": "microsoft.graph.userRegistrationCount"
        }
      ]
    }
  ]
}
```

