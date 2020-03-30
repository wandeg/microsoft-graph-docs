---
title: "List deviceStatuses"
description: "Get the mobileAppInstallStatuses from the deviceStatuses navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceStatuses

Namespace: microsoft.graph

Get the mobileAppInstallStatuses from the deviceStatuses navigation property.

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
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileappinstallstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileappinstallstatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
      "id": "4c36b804-b804-4c36-04b8-364c04b8364c",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:01:32.4757974+03:00",
      "mobileAppInstallStatusValue": "String",
      "installState": "String",
      "installStateDetail": "String",
      "errorCode": 9,
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "displayVersion": "Display Version value"
    }
  ]
}
```

