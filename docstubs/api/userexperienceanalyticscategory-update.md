---
title: "Update userExperienceAnalyticsCategory"
description: "Update the properties of a userExperienceAnalyticsCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userExperienceAnalyticsCategory

Namespace: microsoft.graph

Update the properties of a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticscategory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
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
Content-Length: 530

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "2bb6a47d-a47d-2bb6-7da4-b62b7da4b62b",
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
```

