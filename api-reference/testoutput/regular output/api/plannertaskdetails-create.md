---
title: "Create plannerTaskDetails"
description: "Create a new plannerTaskDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create plannerTaskDetails

Namespace: microsoft.graph

Create a new [plannerTaskDetails](../resources/plannertaskdetails.md) object.

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
POST ** Collection URI for microsoft.graph.plannerTaskDetails not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [plannerTaskDetails](../resources/plannertaskdetails.md) object.

The following table shows the properties that are required when you create the [plannerTaskDetails](../resources/plannertaskdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|references|[plannerExternalReferences](../resources/plannerexternalreferences.md)||
|checklist|[plannerChecklistItems](../resources/plannerchecklistitems.md)||



## Response
If successful, this method returns a `201 Created` response code and a [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannertaskdetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.plannerTaskDetails not found
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannertaskdetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "id": "b8ffec12-ec12-b8ff-12ec-ffb812ecffb8",
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

