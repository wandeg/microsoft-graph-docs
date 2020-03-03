---
title: "Update azureADLicenseUsage"
description: "Update the properties of a azureADLicenseUsage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update azureADLicenseUsage

Namespace: microsoft.graph

Update the properties of a [azureADLicenseUsage](../resources/azureadlicenseusage.md) object.

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
PATCH ** Entity URI for microsoft.graph.azureADLicenseUsage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [azureADLicenseUsage](../resources/azureadlicenseusage.md) object.

The following table shows the properties that are required when you create the [azureADLicenseUsage](../resources/azureadlicenseusage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|snapshotDateTime|DateTimeOffset||
|licenseInfoDetails|[licenseInfoDetail](../resources/licenseinfodetail.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [azureADLicenseUsage](../resources/azureadlicenseusage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_azureadlicenseusage"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.azureADLicenseUsage not found
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.azureADLicenseUsage",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

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
```

