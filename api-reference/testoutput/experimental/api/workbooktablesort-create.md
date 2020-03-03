---
title: "Create workbookTableSort"
description: "Create a new workbookTableSort object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookTableSort

Namespace: microsoft.graph

Create a new [workbookTableSort](../resources/workbooktablesort.md) object.

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
POST ** Collection URI for microsoft.graph.workbookTableSort not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookTableSort](../resources/workbooktablesort.md) object.

The following table shows the properties that are required when you create the [workbookTableSort](../resources/workbooktablesort.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|fields|[workbookSortField](../resources/workbooksortfield.md) collection||
|matchCase|Boolean||
|method|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookTableSort](../resources/workbooktablesort.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbooktablesort_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookTableSort not found
Content-type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField",
      "ascending": true,
      "color": "Color value",
      "dataOption": "Data Option value",
      "icon": {
        "@odata.type": "microsoft.graph.workbookIcon",
        "index": 5,
        "set": "Set value"
      },
      "key": 3,
      "sortOn": "Sort On value"
    }
  ],
  "matchCase": true,
  "method": "Method value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooktablesort"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 534

{
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "id": "320c8dc2-8dc2-320c-c28d-0c32c28d0c32",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField",
      "ascending": true,
      "color": "Color value",
      "dataOption": "Data Option value",
      "icon": {
        "@odata.type": "microsoft.graph.workbookIcon",
        "index": 5,
        "set": "Set value"
      },
      "key": 3,
      "sortOn": "Sort On value"
    }
  ],
  "matchCase": true,
  "method": "Method value"
}
```

