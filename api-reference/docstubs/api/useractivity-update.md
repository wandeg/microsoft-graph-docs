---
title: "Update userActivity"
description: "Update the properties of a userActivity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userActivity

Namespace: microsoft.graph

Update the properties of a [userActivity](../resources/useractivity.md) object.

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
PATCH /me/activities/{userActivityId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [userActivity](../resources/useractivity.md) object.

The following table shows the properties that are required when you create the [userActivity](../resources/useractivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|visualElements|[visualInfo](../resources/visualinfo.md)|**TODO: Add Description**|
|activitySourceHost|String|**TODO: Add Description**|
|activationUrl|String|**TODO: Add Description**|
|appActivityId|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|fallbackUrl|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|userTimezone|String|**TODO: Add Description**|
|contentInfo|[Json](../resources/json.md)|**TODO: Add Description**|
|status|status|**TODO: Add Description**. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [userActivity](../resources/useractivity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_useractivity"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/activities/{userActivityId}
Content-Type: application/json
Content-length: 1102

{
  "@odata.type": "#microsoft.graph.userActivity",
  "visualElements": {
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
      "@odata.type": "microsoft.graph.imageInfo",
      "iconUrl": "https://example.com/iconUrl/",
      "alternativeText": "Alternative Text value",
      "alternateText": "Alternate Text value",
      "addImageQuery": true
    },
    "backgroundColor": "Background Color value",
    "description": "Description value",
    "displayText": "Display Text value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  },
  "activitySourceHost": "Activity Source Host value",
  "activationUrl": "https://example.com/activationUrl/",
  "appActivityId": "App Activity Id value",
  "appDisplayName": "App Display Name value",
  "contentUrl": "https://example.com/contentUrl/",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "fallbackUrl": "https://example.com/fallbackUrl/",
  "userTimezone": "User Timezone value",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userActivity",
  "id": "cc922c74-2c74-cc92-742c-92cc742c92cc",
  "visualElements": {
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
      "@odata.type": "microsoft.graph.imageInfo",
      "iconUrl": "https://example.com/iconUrl/",
      "alternativeText": "Alternative Text value",
      "alternateText": "Alternate Text value",
      "addImageQuery": true
    },
    "backgroundColor": "Background Color value",
    "description": "Description value",
    "displayText": "Display Text value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  },
  "activitySourceHost": "Activity Source Host value",
  "activationUrl": "https://example.com/activationUrl/",
  "appActivityId": "App Activity Id value",
  "appDisplayName": "App Display Name value",
  "contentUrl": "https://example.com/contentUrl/",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "fallbackUrl": "https://example.com/fallbackUrl/",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "userTimezone": "User Timezone value",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

