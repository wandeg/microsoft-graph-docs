---
title: "Create windowsFeatureUpdateProfiles"
description: "Create a new windowsFeatureUpdateProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windowsFeatureUpdateProfiles

Namespace: microsoft.graph

Create a new windowsFeatureUpdateProfiles object.

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
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.

The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The display name of the profile.|
|description|String|The description of the profile which is specified by the user.|
|featureUpdateVersion|String|The feature update version that will be deployed to the devices targeted by this profile. The version could be any supported version for example 1709, 1803 or 1809 and so on.|
|createdDateTime|DateTimeOffset|The date time that the profile was created.|
|lastModifiedDateTime|DateTimeOffset|The date time that the profile was last modified.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsfeatureupdateprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
Content-Type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsfeatureupdateprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "cf3082e7-82e7-cf30-e782-30cfe78230cf",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

