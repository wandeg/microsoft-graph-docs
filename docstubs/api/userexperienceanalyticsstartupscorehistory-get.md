---
title: "Get userExperienceAnalyticsStartupScoreHistory"
description: "Read properties and relationships of the userExperienceAnalyticsStartupScoreHistory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userExperienceAnalyticsStartupScoreHistory

Namespace: microsoft.graph

Read properties and relationships of the [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object.

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
GET /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsstartupscorehistory"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userExperienceAnalyticsStartupScoreHistory"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
    "id": "f9a163a8-63a8-f9a1-a863-a1f9a863a1f9",
    "startupDateTime": "2017-01-01T00:01:26.0817508+03:00"
  }
}
```

