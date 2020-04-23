---
title: "Create details"
description: "Create a new details object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create details

Namespace: microsoft.graph

Create a new details object.

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
POST /invitations/{invitationsId}/invitedUser/planner/tasks/{plannerTaskId}/details
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannertaskdetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/planner/tasks/{plannerTaskId}/details
Content-Type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "description": "Description value",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.plannertaskdetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "id": "51554836-4836-5155-3648-555136485551",
  "description": "Description value",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
}
```

