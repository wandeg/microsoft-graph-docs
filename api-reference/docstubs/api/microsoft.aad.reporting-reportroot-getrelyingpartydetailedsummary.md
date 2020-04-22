---
title: "reportRoot: getRelyingPartyDetailedSummary"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# getRelyingPartyDetailedSummary

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
GET /reports/getRelyingPartyDetailedSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [relyingPartyDetailedSummary](../resources/microsoft.aad.reporting-relyingpartydetailedsummary.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getrelyingpartydetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.relyingpartydetailedsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.relyingPartyDetailedSummary",
      "id": "ea51dda1-dda1-ea51-a1dd-51eaa1dd51ea",
      "relyingPartyId": "Relying Party Id value",
      "serviceId": "Service Id value",
      "relyingPartyName": "Relying Party Name value",
      "successfulSignInCount": 5,
      "failedSignInCount": 1,
      "totalSignInCount": 0,
      "signInSuccessRate": "Double",
      "uniqueUserCount": 15,
      "migrationStatus": "String",
      "migrationValidationDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.keyValuePair"
        }
      ],
      "replyUrls": [
        "Reply Urls value"
      ]
    }
  ]
}
```

