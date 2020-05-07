---
title: "Create deviceUpdateStates"
description: "Create a new deviceUpdateStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceUpdateStates

Namespace: microsoft.graph

Create a new deviceUpdateStates object.

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
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/deviceUpdateStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsUpdateState](../resources/windowsupdatestate.md) object.

The following table shows the properties that are required when you create the [windowsUpdateState](../resources/windowsupdatestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|deviceDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|status|windowsUpdateStatus|**TODO: Add Description**. Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|String|**TODO: Add Description**|
|featureUpdateVersion|String|**TODO: Add Description**|
|lastScanDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/windowsupdatestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsupdatestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/deviceUpdateStates
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsupdatestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "a2649f57-9f57-a264-579f-64a2579f64a2",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```

