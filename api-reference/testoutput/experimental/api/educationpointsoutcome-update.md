---
title: "Update educationPointsOutcome"
description: "Update the properties of a educationPointsOutcome object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationPointsOutcome

Update the properties of a [educationPointsOutcome](../resources/educationpointsoutcome.md) object.

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
PATCH ** Entity URI for microsoft.graph.educationPointsOutcome not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [educationPointsOutcome](../resources/educationPointsOutcome.md) object.

The following table shows the properties that are required when you create the [educationPointsOutcome](../resources/educationpointsoutcome.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|points|[educationAssignmentPointsGrade](../resources/educationAssignmentPointsGrade.md)||
|publishedPoints|[educationAssignmentPointsGrade](../resources/educationAssignmentPointsGrade.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationPointsOutcome](../resources/educationpointsoutcome.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.educationPointsOutcome not found
Content-type: application/json
Content-length: 417

{
  "@odata.type": "#microsoft.graph.educationPointsOutcome",
  "points": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade",
    "gradedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2017-01-01T00:02:25.6674094+03:00",
    "points": "Single"
  },
  "publishedPoints": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 903

{
  "@odata.type": "#microsoft.graph.educationPointsOutcome",
  "id": "eb98b7f1-b7f1-eb98-f1b7-98ebf1b798eb",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "points": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade",
    "gradedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2017-01-01T00:02:25.6674094+03:00",
    "points": "Single"
  },
  "publishedPoints": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
  }
}
```

