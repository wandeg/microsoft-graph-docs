---
title: "reportRoot: getAzureADLicenseUsage"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getAzureADLicenseUsage

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
GET /reports/getAzureADLicenseUsage
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [azureADLicenseUsage](../resources/microsoft.aad.reporting-azureadlicenseusage.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getazureadlicenseusage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAzureADLicenseUsage(period='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.azureadlicenseusage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.azureADLicenseUsage",
      "id": "0e602c49-2c49-0e60-492c-600e492c600e",
      "snapshotDateTime": "2016-12-31T23:59:52.9238491+00:00",
      "licenseInfoDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.licenseInfoDetail"
        }
      ]
    }
  ]
}
```

