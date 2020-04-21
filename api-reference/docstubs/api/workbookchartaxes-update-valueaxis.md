---
title: "Update valueAxis"
description: "Update the properties of a valueAxis object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update valueAxis

Namespace: microsoft.graph

Update the properties of a valueAxis object.

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
PATCH /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/valueAxis
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxis](../resources/workbookchartaxis.md) object.

The following table shows the properties that are required when you create the [workbookChartAxis](../resources/workbookchartaxis.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|majorUnit|[Json](../resources/json.md)|**TODO: Add Description**|
|maximum|[Json](../resources/json.md)|**TODO: Add Description**|
|minimum|[Json](../resources/json.md)|**TODO: Add Description**|
|minorUnit|[Json](../resources/json.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartAxis](../resources/workbookchartaxis.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_valueaxis"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/valueAxis
Content-Type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "id": "bf864c14-4c14-bf86-144c-86bf144c86bf",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

