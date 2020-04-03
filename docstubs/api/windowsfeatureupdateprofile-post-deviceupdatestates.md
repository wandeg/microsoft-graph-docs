---
title: "Add deviceUpdateStates"
description: "Add deviceUpdateStates by posting to the deviceUpdateStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceUpdateStates

Namespace: microsoft.graph

Add deviceUpdateStates by posting to the deviceUpdateStates collection.

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
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/deviceUpdateStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [windowsUpdateState](../resources/windowsupdatestate.md) object.

The following table shows the properties that are required when you create the [windowsUpdateState](../resources/windowsupdatestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceId|String||
|userId|String||
|deviceDisplayName|String||
|userPrincipalName|String||
|status|Enumeration| Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|String||
|featureUpdateVersion|String||
|lastScanDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/windowsupdatestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsupdatestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/deviceUpdateStates
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsupdatestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 540

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
```

