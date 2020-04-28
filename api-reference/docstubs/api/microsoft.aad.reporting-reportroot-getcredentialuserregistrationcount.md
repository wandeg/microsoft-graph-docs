---
title: "reportRoot: getCredentialUserRegistrationCount"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# getCredentialUserRegistrationCount

Namespace: Microsoft.AAD.Reporting

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
GET /reports/getCredentialUserRegistrationCount
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [credentialUserRegistrationCount](../resources/microsoft.aad.reporting-credentialuserregistrationcount.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.credentialuserregistrationcount)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.credentialUserRegistrationCount",
      "id": "b14a04ab-04ab-b14a-ab04-4ab1ab044ab1",
      "totalUserCount": 14,
      "userRegistrationCounts": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.userRegistrationCount"
        }
      ]
    }
  ]
}
```

