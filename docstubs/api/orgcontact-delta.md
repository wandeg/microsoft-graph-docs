---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

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
GET /contacts/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [orgContact](../resources/orgcontact.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/contacts/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.orgcontact)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1070

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "1cd20d64-0d64-1cd2-640d-d21c640dd21c",
      "deletedDateTime": "2016-12-31T23:58:43.3543606+03:00",
      "addresses": [
        {
          "@odata.type": "microsoft.graph.physicalOfficeAddress"
        }
      ],
      "companyName": "Company Name value",
      "department": "Department value",
      "displayName": "Display Name value",
      "givenName": "Given Name value",
      "jobTitle": "Job Title value",
      "mail": "Mail value",
      "mailNickname": "Mail Nickname value",
      "onPremisesSyncEnabled": true,
      "onPremisesLastSyncDateTime": "2016-12-31T23:56:34.7560821+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError"
        }
      ],
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone"
        }
      ],
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "surname": "Surname value"
    }
  ]
}
```

