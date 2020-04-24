---
title: "List filter"
description: "Get the workbookFilters from the filter navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List filter

Namespace: microsoft.graph

Get the workbookFilters from the filter navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookFilter](../resources/workbookfilter.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbookfilter"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookfilter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookFilter",
      "id": "f14f34bc-34bc-f14f-bc34-4ff1bc344ff1",
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
  ]
}
```

