---
title: "Add app"
description: "Add app by posting to the app collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add app

Namespace: microsoft.graph

Add app by posting to the app collection.

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mobileApp](../resources/mobileapp.md) object.

The following table shows the properties that are required when you create the [mobileApp](../resources/mobileapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|largeIcon|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|isFeatured|Boolean|**TODO: Add Description**|
|privacyInformationUrl|String|**TODO: Add Description**|
|informationUrl|String|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|developer|String|**TODO: Add Description**|
|notes|String|**TODO: Add Description**|
|uploadState|Int32|**TODO: Add Description**|
|publishingState|mobileAppPublishingState|**TODO: Add Description**. Possible values are: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|dependentAppCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [mobileApp](../resources/mobileapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_mobileapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/$ref
Content-Type: application/json
Content-length: 542

{
  "@odata.type": "#microsoft.graph.mobileApp",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "isFeatured": "Boolean",
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": "Integer",
  "publishingState": "String",
  "isAssigned": "Boolean",
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileapp"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "3d4ec2ba-c2ba-3d4e-bac2-4e3dbac24e3d",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": "Boolean",
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": "Integer",
  "publishingState": "String",
  "isAssigned": "Boolean",
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": "Integer"
}
```

