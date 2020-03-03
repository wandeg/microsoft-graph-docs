---
title: "Add assignmentCategories"
description: "Add assignmentCategories by posting to the assignmentCategories collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add assignmentCategories

Namespace: microsoft.graph

Add assignmentCategories by posting to the assignmentCategories collection.

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
POST /education/classes/{educationClassId}/assignmentCategories/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [educationCategory](../resources/educationcategory.md) object.

The following table shows the properties that are required when you create the [educationCategory](../resources/educationcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/education/classes/{educationClassId}/assignmentCategories
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
  "truncated": true,
  "@odata.type": "microsoft.graph.educationcategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 148

{
  "@odata.type": "#microsoft.graph.educationCategory",
  "id": "be0967cb-67cb-be09-cb67-09becb6709be",
  "displayName": "Display Name value"
}
```

