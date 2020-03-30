---
title: "List userExperienceAnalyticsStartupScoreHistory"
description: "Get the userExperienceAnalyticsStartupScoreHistories from the userExperienceAnalyticsStartupScoreHistory navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userExperienceAnalyticsStartupScoreHistory

Namespace: microsoft.graph

Get the userExperienceAnalyticsStartupScoreHistories from the userExperienceAnalyticsStartupScoreHistory navigation property.

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
GET /deviceManagement/userExperienceAnalyticsStartupScoreHistory
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
If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsstartupscorehistory"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userexperienceanalyticsstartupscorehistory)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
      "id": "9d3b01a7-01a7-9d3b-a701-3b9da7013b9d",
      "startupDateTime": "2016-12-31T23:56:51.9148226+03:00"
    }
  ]
}
```

