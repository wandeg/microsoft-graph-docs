---
title: "Get details"
description: "Read the properties and relationships of a plannerTaskDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get details

Namespace: microsoft.graph

Read the properties and relationships of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/planner/tasks/{plannerTaskId}/details
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/planner/tasks/{plannerTaskId}/details
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.plannerTaskDetails",
    "id": "ef4fce74-ce74-ef4f-74ce-4fef74ce4fef",
    "description": "String",
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

