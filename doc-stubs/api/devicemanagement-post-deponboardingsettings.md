---
title: "Create depOnboardingSettings"
description: "Create a new depOnboardingSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create depOnboardingSettings

Namespace: microsoft.graph

Create a new depOnboardingSettings object.

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
POST /deviceManagement/depOnboardingSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [depOnboardingSetting](../resources/deponboardingsetting.md) object.

The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/deponboardingsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appleIdentifier|String|**TODO: Add Description**|
|tokenExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSuccessfulSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncTriggeredDateTime|DateTimeOffset|**TODO: Add Description**|
|shareTokenWithSchoolDataSyncService|Boolean|**TODO: Add Description**|
|lastSyncErrorCode|Int32|**TODO: Add Description**|
|tokenType|depTokenType|**TODO: Add Description**. Possible values are: `none`, `dep`, `appleSchoolManager`.|
|tokenName|String|**TODO: Add Description**|
|syncedDeviceCount|Int32|**TODO: Add Description**|
|dataSharingConsentGranted|Boolean|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/deponboardingsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deponboardingsetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-Type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": "Boolean",
  "lastSyncErrorCode": "Integer",
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": "Integer",
  "dataSharingConsentGranted": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deponboardingsetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "8c645e2d-5e2d-8c64-2d5e-648c2d5e648c",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": "Boolean",
  "lastSyncErrorCode": "Integer",
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": "Integer",
  "dataSharingConsentGranted": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

