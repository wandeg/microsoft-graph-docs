---
title: "Create educationPointsOutcome"
description: "Create a new educationPointsOutcome object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create educationPointsOutcome

Create a new [educationPointsOutcome](../resources/educationpointsoutcome.md) object.

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
POST ** Collection URI for microsoft.graph.educationPointsOutcome not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the educationPointsOutcome object.

The following table shows the properties that are required when you create the educationPointsOutcome.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|points|[educationAssignmentPointsGrade](../resources/educationAssignmentPointsGrade.md)||
|publishedPoints|[educationAssignmentPointsGrade](../resources/educationAssignmentPointsGrade.md)||



## Response
If successful, this method returns a `201 Created` response code and a [educationPointsOutcome](../resources/educationpointsoutcome.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationpointsoutcome_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.educationPointsOutcome not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.educationpointsoutcome"
}
-->
``` http
HTTP/1.1 201 Created
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

