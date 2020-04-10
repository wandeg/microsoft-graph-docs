---
title: "Update windowsProtectionState"
description: "Update the properties of a windowsProtectionState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsProtectionState

Namespace: microsoft.graph

Update the properties of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.

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
PATCH /me/managedDevices/{managedDeviceId}/windowsProtectionState
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsProtectionState](../resources/windowsprotectionstate.md) object.

The following table shows the properties that are required when you create the [windowsProtectionState](../resources/windowsprotectionstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|malwareProtectionEnabled|Boolean||
|deviceState|Enumeration| Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Boolean||
|networkInspectionSystemEnabled|Boolean||
|quickScanOverdue|Boolean||
|fullScanOverdue|Boolean||
|signatureUpdateOverdue|Boolean||
|rebootRequired|Boolean||
|fullScanRequired|Boolean||
|engineVersion|String||
|signatureVersion|String||
|antiMalwareVersion|String||
|lastQuickScanDateTime|DateTimeOffset||
|lastFullScanDateTime|DateTimeOffset||
|lastQuickScanSignatureVersion|String||
|lastFullScanSignatureVersion|String||
|lastReportedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/windowsprotectionstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windowsprotectionstate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/windowsProtectionState
Content-type: application/json
Content-length: 856

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:04.0946323+00:00",
  "lastFullScanDateTime": "2016-12-31T23:57:57.8180934+00:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2016-12-31T23:59:48.2289145+00:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 905

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "5d4c7932-7932-5d4c-3279-4c5d32794c5d",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:04.0946323+00:00",
  "lastFullScanDateTime": "2016-12-31T23:57:57.8180934+00:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2016-12-31T23:59:48.2289145+00:00"
}
```

