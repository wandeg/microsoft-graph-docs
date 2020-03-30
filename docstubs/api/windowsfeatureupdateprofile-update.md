---
title: "Update windowsFeatureUpdateProfile"
description: "Update the properties of a windowsFeatureUpdateProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsFeatureUpdateProfile

Namespace: microsoft.graph

Update the properties of a [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.

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
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.

The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|featureUpdateVersion|String||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsfeatureupdateprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value"
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
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "d26a6467-6467-d26a-6764-6ad267646ad2",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00"
}
```

