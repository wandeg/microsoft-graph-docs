---
title: "List mobileAppInstallSummaries"
description: "List properties and relationships of the mobileAppInstallSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mobileAppInstallSummaries

Namespace: microsoft.graph

List properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) objects.

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
GET ** Collection URI for microsoft.graph.mobileAppInstallSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileappinstallsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.mobileAppInstallSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileappinstallsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
      "id": "71932d78-2d78-7193-782d-9371782d9371",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notApplicableDeviceCount": 8,
      "notInstalledDeviceCount": 7,
      "pendingInstallDeviceCount": 9,
      "installedUserCount": 2,
      "failedUserCount": 15,
      "notApplicableUserCount": 6,
      "notInstalledUserCount": 5,
      "pendingInstallUserCount": 7
    }
  ]
}
```

