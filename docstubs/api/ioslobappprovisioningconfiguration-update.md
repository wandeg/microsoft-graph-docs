---
title: "Update iosLobAppProvisioningConfiguration"
description: "Update the properties of a iosLobAppProvisioningConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update iosLobAppProvisioningConfiguration

Namespace: microsoft.graph

Update the properties of a [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.

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
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.

The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|expirationDateTime|DateTimeOffset||
|payloadFileName|String||
|payload|Binary||
|roleScopeTagIds|String collection||
|createdDateTime|DateTimeOffset||
|description|String||
|lastModifiedDateTime|DateTimeOffset||
|displayName|String||
|version|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_ioslobappprovisioningconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
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
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "57c069f7-69f7-57c0-f769-c057f769c057",
  "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "description": "Description value",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "displayName": "Display Name value",
  "version": 7
}
```

