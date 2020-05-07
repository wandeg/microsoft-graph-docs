---
title: "teamwork: generateActivityNotification"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# generateActivityNotification

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /teamwork/generateActivityNotification
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|about|String|**TODO: Add Description**|
|activityType|String|**TODO: Add Description**|
|aggregationId|Int64|**TODO: Add Description**|
|onClickWebUrl|String|**TODO: Add Description**|
|previewText|String|**TODO: Add Description**|
|teamsAppId|String|**TODO: Add Description**|
|templateParameters|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|recipient|[teamworkNotificationAudience](../resources/teamworknotificationaudience.md)|**TODO: Add Description**|



## Response

If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "teamwork_generateactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamwork/generateActivityNotification

Content-Type: application/json
Content-length: 360

{
  "about": "String",
  "activityType": "String",
  "aggregationId": "Integer",
  "onClickWebUrl": "String",
  "previewText": "String",
  "teamsAppId": "String",
  "templateParameters": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "recipient": {
    "@odata.type": "microsoft.graph.aadUserNotificationAudience"
  }
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
HTTP/1.1 204 No Content
```

