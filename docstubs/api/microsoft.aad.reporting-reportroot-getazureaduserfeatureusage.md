---
title: "reportRoot: getAzureADUserFeatureUsage"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getAzureADUserFeatureUsage

Namespace: Microsoft.AAD.Reporting



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
GET /reports/getAzureADUserFeatureUsage
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [azureADUserFeatureUsage](../resources/microsoft.aad.reporting-azureaduserfeatureusage.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getazureaduserfeatureusage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAzureADUserFeatureUsage
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.azureaduserfeatureusage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 584

{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.azureADUserFeatureUsage",
      "id": "04a04e96-4e96-04a0-964e-a004964ea004",
      "lastUpdatedDateTime": "2016-12-31T23:59:13.0235347+00:00",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "licenseRecommended": "String",
      "licenseAssigned": "String",
      "featureUsageDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.featureUsageDetail"
        }
      ]
    }
  ]
}
```

