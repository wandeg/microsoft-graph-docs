---
title: "Update userExperienceAnalyticsStartupScoreHistory"
description: "Update the properties of a userExperienceAnalyticsStartupScoreHistory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userExperienceAnalyticsStartupScoreHistory

Namespace: microsoft.graph

Update the properties of a [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|startupDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsstartupscorehistory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
Content-type: application/json
Content-length: 143

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "startupDateTime": "2017-01-01T00:03:15.3456965+00:00"
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
Content-Length: 192

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "372eb7de-b7de-372e-deb7-2e37deb72e37",
  "startupDateTime": "2017-01-01T00:03:15.3456965+00:00"
}
```

