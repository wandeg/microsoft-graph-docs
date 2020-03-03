---
title: "Get plannerTaskDetails"
description: "Read properties and relationships of the plannerTaskDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get plannerTaskDetails

Namespace: microsoft.graph

Read properties and relationships of the [plannerTaskDetails](../resources/plannertaskdetails.md) object.

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
GET /me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/details
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/details
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 388

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerTaskDetails",
    "id": "b27fecb6-ecb6-b27f-b6ec-7fb2b6ec7fb2",
    "description": "Description value",
    "previewType": "String",
    "references": {
      "@odata.type": "microsoft.graph.plannerExternalReferences"
    },
    "checklist": {
      "@odata.type": "microsoft.graph.plannerChecklistItems"
    }
  }
}
```

