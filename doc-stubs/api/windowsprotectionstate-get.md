---
title: "Get windowsProtectionState"
description: "Read the properties and relationships of a windowsProtectionState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get windowsProtectionState

Namespace: microsoft.graph

Read the properties and relationships of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.

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
GET /me/managedDevices/{managedDeviceId}/windowsProtectionState
GET /users/{usersId}/managedDevices/{managedDeviceId}/windowsProtectionState
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
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

If successful, this method returns a `200 OK` response code and a [windowsProtectionState](../resources/windowsprotectionstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/windowsProtectionState
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "208f58d2-58d2-208f-d258-8f20d2588f20",
    "malwareProtectionEnabled": "Boolean",
    "deviceState": "String",
    "realTimeProtectionEnabled": "Boolean",
    "networkInspectionSystemEnabled": "Boolean",
    "quickScanOverdue": "Boolean",
    "fullScanOverdue": "Boolean",
    "signatureUpdateOverdue": "Boolean",
    "rebootRequired": "Boolean",
    "fullScanRequired": "Boolean",
    "engineVersion": "String",
    "signatureVersion": "String",
    "antiMalwareVersion": "String",
    "lastQuickScanDateTime": "String (timestamp)",
    "lastFullScanDateTime": "String (timestamp)",
    "lastQuickScanSignatureVersion": "String",
    "lastFullScanSignatureVersion": "String",
    "lastReportedDateTime": "String (timestamp)"
  }
}
```

