---
title: "List userExperienceAnalyticsOverviews"
description: "List properties and relationships of the userExperienceAnalyticsOverview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userExperienceAnalyticsOverviews

List properties and relationships of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.userExperienceAnalyticsOverview not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsoverview"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.userExperienceAnalyticsOverview not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userexperienceanalyticsoverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
      "id": "273bb623-b623-273b-23b6-3b2723b63b27",
      "insights": [
        {
          "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
          "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
          "insightId": "Insight Id value",
          "values": [
            {
              "@odata.type": "microsoft.graph.insightValueDouble",
              "value": "Double"
            }
          ],
          "severity": "String"
        }
      ]
    }
  ]
}
```

