---
title: "Update details"
description: "Update the properties of a details object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update details

Namespace: microsoft.graph

Update the properties of a details object.

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
PATCH /users/{usersId}/planner/tasks/{plannerTaskId}/details
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerTaskDetails](../resources/plannertaskdetails.md) object.

The following table shows the properties that are required when you create the [plannerTaskDetails](../resources/plannertaskdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|previewType|plannerPreviewType|**TODO: Add Description**. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|references|[plannerExternalReferences](../resources/plannerexternalreferences.md)|**TODO: Add Description**|
|checklist|[plannerChecklistItems](../resources/plannerchecklistitems.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_details"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/planner/tasks/{plannerTaskId}/details
Content-Type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "description": "String",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "id": "e2685b44-5b44-e268-445b-68e2445b68e2",
  "description": "String",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
}
```

