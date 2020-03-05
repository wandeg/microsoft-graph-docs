---
title: "Create workbookChartSeriesFormat"
description: "Create a new workbookChartSeriesFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartSeriesFormat

Namespace: microsoft.graph

Create a new [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartSeriesFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.

The following table shows the properties that are required when you create the [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartseriesformat_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartSeriesFormat not found
Content-type: application/json
Content-length: 67

{
  "@odata.type": "#microsoft.graph.workbookChartSeriesFormat"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartseriesformat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 116

{
  "@odata.type": "#microsoft.graph.workbookChartSeriesFormat",
  "id": "035afda4-fda4-035a-a4fd-5a03a4fd5a03"
}
```

