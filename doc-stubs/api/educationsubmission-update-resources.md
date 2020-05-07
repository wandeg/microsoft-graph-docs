---
title: "Update resources"
description: "Update the properties of a resources object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update resources

Namespace: microsoft.graph

Update the properties of a resources object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/resources
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.

The following table shows the properties that are required when you create the [educationSubmissionResource](../resources/educationsubmissionresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resource|[educationResource](../resources/educationresource.md)|**TODO: Add Description**|
|assignmentResourceUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_resources"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/resources
Content-Type: application/json
Content-length: 186

{
  "@odata.type": "#microsoft.graph.educationSubmissionResource",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  },
  "assignmentResourceUrl": "String"
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
  "@odata.type": "#microsoft.graph.educationSubmissionResource",
  "id": "360b5d06-5d06-360b-065d-0b36065d0b36",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  },
  "assignmentResourceUrl": "String"
}
```

