---
title: "Update educationCategory"
description: "Update the properties of a educationCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationCategory

Namespace: microsoft.graph

Update the properties of a [educationCategory](../resources/educationcategory.md) object.

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
PATCH /education/classes/{educationClassId}/assignmentCategories/{educationCategoryId}
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/categories/{educationCategoryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationCategory](../resources/educationcategory.md) object.

The following table shows the properties that are required when you create the [educationCategory](../resources/educationcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationCategory](../resources/educationcategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationcategory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignmentCategories/{educationCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.educationCategory",
  "displayName": "Display Name value"
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
Content-Length: 148

{
  "@odata.type": "#microsoft.graph.educationCategory",
  "id": "fae63cc6-3cc6-fae6-c63c-e6fac63ce6fa",
  "displayName": "Display Name value"
}
```

