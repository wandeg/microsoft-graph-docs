---
title: "List deviceStatuses"
description: "Get the mobileAppInstallStatus from the deviceStatuses navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceStatuses

Namespace: microsoft.graph

Get the mobileAppInstallStatus from the deviceStatuses navigation property.

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
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mobileappinstallstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileappinstallstatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
      "id": "fdc9ede3-ede3-fdc9-e3ed-c9fde3edc9fd",
      "deviceName": "String",
      "deviceId": "String",
      "lastSyncDateTime": "String (timestamp)",
      "mobileAppInstallStatusValue": "String",
      "installState": "String",
      "installStateDetail": "String",
      "errorCode": "Integer",
      "osVersion": "String",
      "osDescription": "String",
      "userName": "String",
      "userPrincipalName": "String",
      "displayVersion": "String"
    }
  ]
}
```

