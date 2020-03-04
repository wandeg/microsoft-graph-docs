---
title: "Create workbookChartLegend"
description: "Create a new workbookChartLegend object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartLegend

Namespace: microsoft.graph

Create a new [workbookChartLegend](../resources/workbookchartlegend.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartLegend not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartLegend](../resources/workbookchartlegend.md) object.

The following table shows the properties that are required when you create the [workbookChartLegend](../resources/workbookchartlegend.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|position|String||
|visible|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartlegend_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartLegend not found
Content-type: application/json
Content-length: 134

{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "overlay": true,
  "position": "Position value",
  "visible": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartlegend"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 183

{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "id": "acd13583-3583-acd1-8335-d1ac8335d1ac",
  "overlay": true,
  "position": "Position value",
  "visible": true
}
```

