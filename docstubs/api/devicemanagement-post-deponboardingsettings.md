---
title: "Add depOnboardingSettings"
description: "Add depOnboardingSettings by posting to the depOnboardingSettings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add depOnboardingSettings

Namespace: microsoft.graph

Add depOnboardingSettings by posting to the depOnboardingSettings collection.

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
POST /deviceManagement/depOnboardingSettings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/deponboardingsetting.md) object.

The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/deponboardingsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appleIdentifier|String||
|tokenExpirationDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|lastSuccessfulSyncDateTime|DateTimeOffset||
|lastSyncTriggeredDateTime|DateTimeOffset||
|shareTokenWithSchoolDataSyncService|Boolean||
|lastSyncErrorCode|Int32||
|tokenType|Enumeration| Possible values are: `none`, `dep`, `appleSchoolManager`.|
|tokenName|String||
|syncedDeviceCount|Int32||
|dataSharingConsentGranted|Boolean||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/deponboardingsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deponboardingsetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 579

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2017-01-01T00:02:47.1539709+03:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:00:12.5003892+03:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:15.235494+03:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "String",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deponboardingsetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 692

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "6c0a9333-9333-6c0a-3393-0a6c33930a6c",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2017-01-01T00:02:47.1539709+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:00:12.5003892+03:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:15.235494+03:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "String",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

