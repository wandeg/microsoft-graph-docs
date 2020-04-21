---
title: "Create filter"
description: "Create a new filter object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create filter

Namespace: microsoft.graph

Create a new filter object.

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
POST /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [workbookFilter](../resources/workbookfilter.md) object.

The following table shows the properties that are required when you create the [workbookFilter](../resources/workbookfilter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|criteria|[workbookFilterCriteria](../resources/workbookfiltercriteria.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [workbookFilter](../resources/workbookfilter.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookfilter_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
Content-Type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria",
    "color": "Color value",
    "criterion1": "Criterion1 value",
    "criterion2": "Criterion2 value",
    "dynamicCriteria": "Dynamic Criteria value",
    "filterOn": "Filter On value",
    "icon": {
      "@odata.type": "microsoft.graph.workbookIcon",
      "index": 5,
      "set": "Set value"
    },
    "operator": "Operator value",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookfilter"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "6e32a69f-a69f-6e32-9fa6-326e9fa6326e",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria",
    "color": "Color value",
    "criterion1": "Criterion1 value",
    "criterion2": "Criterion2 value",
    "dynamicCriteria": "Dynamic Criteria value",
    "filterOn": "Filter On value",
    "icon": {
      "@odata.type": "microsoft.graph.workbookIcon",
      "index": 5,
      "set": "Set value"
    },
    "operator": "Operator value",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

