---
title: "Create activities"
description: "Create a new activities object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create activities

Namespace: microsoft.graph

Create a new activities object.

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
POST /me/activities
POST /users/{usersId}/activities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [userActivity](../resources/useractivity.md) object.

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
If successful, this method returns a `201 Created` response code and an [userActivity](../resources/useractivity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_useractivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/activities
Content-Type: application/json
Content-length: 1103

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
  "expirationDateTime": "2016-12-31T23:56:35.7548719+00:00",
  "fallbackUrl": "https://example.com/fallbackUrl/",
  "userTimezone": "User Timezone value",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.useractivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userActivity",
  "id": "6a551cba-1cba-6a55-ba1c-556aba1c556a",
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
  "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
  "expirationDateTime": "2016-12-31T23:56:35.7548719+00:00",
  "fallbackUrl": "https://example.com/fallbackUrl/",
  "lastModifiedDateTime": "2017-01-01T00:01:26.0388723+00:00",
  "userTimezone": "User Timezone value",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

