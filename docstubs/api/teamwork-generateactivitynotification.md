---
title: "generateActivityNotification"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# generateActivityNotification

Namespace: microsoft.graph



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
POST /teamwork/generateActivityNotification
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|about|String||
|activityType|String||
|aggregationId|Int64||
|onClickWebUrl|String||
|previewText|String||
|teamsAppId|String||
|templateParameters|[keyValuePair](../resources/keyvaluepair.md) collection||
|recipient|[teamworkNotificationAudience](../resources/teamworknotificationaudience.md)||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "teamwork_generateactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamwork/generateActivityNotification

Content-type: application/json
Content-length: 515

{
  "about": "About value",
  "activityType": "Activity Type value",
  "aggregationId": 13,
  "onClickWebUrl": "https://example.com/onClickWebUrl/",
  "previewText": "Preview Text value",
  "teamsAppId": "Teams App Id value",
  "templateParameters": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "recipient": {
    "@odata.type": "microsoft.graph.aadUserNotificationAudience",
    "userId": "User Id value"
  }
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
HTTP/1.1 204 No Content
```

