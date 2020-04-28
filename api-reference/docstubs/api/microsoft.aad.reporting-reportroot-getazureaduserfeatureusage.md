---
title: "reportRoot: getAzureADUserFeatureUsage"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# getAzureADUserFeatureUsage

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
GET /reports/getAzureADUserFeatureUsage
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
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
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.azureADUserFeatureUsage",
      "id": "cab56877-6877-cab5-7768-b5ca7768b5ca",
      "lastUpdatedDateTime": "2016-12-31T23:59:55.6446199+00:00",
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

