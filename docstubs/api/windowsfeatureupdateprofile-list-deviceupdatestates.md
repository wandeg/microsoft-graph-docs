---
title: "List deviceUpdateStates"
description: "Get the windowsUpdateStates from the deviceUpdateStates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceUpdateStates

Namespace: microsoft.graph

Get the windowsUpdateStates from the deviceUpdateStates navigation property.

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
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/deviceUpdateStates
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
If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/windowsupdatestate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsupdatestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/deviceUpdateStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsupdatestate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 617

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateState",
      "id": "fbe71e5c-1e5c-fbe7-5c1e-e7fb5c1ee7fb",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "status": "String",
      "qualityUpdateVersion": "Quality Update Version value",
      "featureUpdateVersion": "Feature Update Version value",
      "lastScanDateTime": "2016-12-31T23:57:02.8566658+00:00",
      "lastSyncDateTime": "2016-12-31T23:57:21.5163223+00:00"
    }
  ]
}
```

