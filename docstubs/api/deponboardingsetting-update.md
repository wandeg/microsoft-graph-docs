---
title: "Update depOnboardingSetting"
description: "Update the properties of a depOnboardingSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update depOnboardingSetting

Namespace: microsoft.graph

Update the properties of a [depOnboardingSetting](../resources/deponboardingsetting.md) object.

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/deponboardingsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deponboardingsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 579

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:06.9056119+03:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:00:45.1839032+03:00",
  "lastSyncTriggeredDateTime": "2016-12-31T23:59:06.620772+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 692

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "a63a6c81-6c81-a63a-816c-3aa6816c3aa6",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:06.9056119+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:00:45.1839032+03:00",
  "lastSyncTriggeredDateTime": "2016-12-31T23:59:06.620772+03:00",
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

