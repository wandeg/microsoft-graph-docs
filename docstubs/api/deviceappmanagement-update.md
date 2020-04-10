---
title: "Update deviceAppManagement"
description: "Update the properties of a deviceAppManagement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceAppManagement

Namespace: microsoft.graph

Update the properties of a [deviceAppManagement](../resources/deviceappmanagement.md) object.

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
PATCH /deviceAppManagement
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceAppManagement](../resources/deviceappmanagement.md) object.

The following table shows the properties that are required when you create the [deviceAppManagement](../resources/deviceappmanagement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset||
|isEnabledForMicrosoftStoreForBusiness|Boolean||
|microsoftStoreForBusinessLanguage|String||
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset||
|microsoftStoreForBusinessPortalSelection|Enumeration| Possible values are: `none`, `companyPortal`, `privateStore`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/deviceappmanagement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceappmanagement"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 451

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2017-01-01T00:02:43.7489788+00:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:03:00.3750678+00:00",
  "microsoftStoreForBusinessPortalSelection": "String"
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
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "4ec39110-9110-4ec3-1091-c34e1091c34e",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2017-01-01T00:02:43.7489788+00:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:03:00.3750678+00:00",
  "microsoftStoreForBusinessPortalSelection": "String"
}
```

