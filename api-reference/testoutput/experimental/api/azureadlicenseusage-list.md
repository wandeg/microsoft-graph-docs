---
title: "List azureADLicenseUsages"
description: "List properties and relationships of the azureADLicenseUsage objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List azureADLicenseUsages

Namespace: microsoft.graph

List properties and relationships of the [azureADLicenseUsage](../resources/azureadlicenseusage.md) objects.

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
GET ** Collection URI for microsoft.graph.azureADLicenseUsage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [azureADLicenseUsage](../resources/azureadlicenseusage.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_azureadlicenseusage"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.azureADLicenseUsage not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.azureadlicenseusage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.azureADLicenseUsage",
      "id": "3d61534f-534f-3d61-4f53-613d4f53613d",
      "snapshotDateTime": "2016-12-31T23:56:35.704242+03:00",
      "licenseInfoDetails": [
        {
          "@odata.type": "microsoft.graph.licenseInfoDetail",
          "licenseType": "String",
          "totalLicenseCount": 1,
          "totalAssignedCount": 2,
          "totalUsageCount": 15
        }
      ]
    }
  ]
}
```

