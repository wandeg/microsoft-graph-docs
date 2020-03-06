---
title: "List userExperienceAnalyticsBaselines"
description: "Get the userExperienceAnalyticsBaselines from the userExperienceAnalyticsBaselines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userExperienceAnalyticsBaselines

Namespace: microsoft.graph

Get the userExperienceAnalyticsBaselines from the userExperienceAnalyticsBaselines navigation property.

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
GET /deviceManagement/userExperienceAnalyticsBaselines
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsbaseline"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/userExperienceAnalyticsBaselines
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userexperienceanalyticsbaseline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
      "id": "15ebf4f5-f4f5-15eb-f5f4-eb15f5f4eb15",
      "displayName": "Display Name value",
      "isBuiltIn": true,
      "createdDateTime": "2017-01-01T00:02:14.7219499+03:00"
    }
  ]
}
```

