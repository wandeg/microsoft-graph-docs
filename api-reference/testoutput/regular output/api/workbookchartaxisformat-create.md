---
title: "Create workbookChartAxisFormat"
description: "Create a new workbookChartAxisFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartAxisFormat

Namespace: microsoft.graph

Create a new [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartAxisFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.

The following table shows the properties that are required when you create the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartaxisformat_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartAxisFormat not found
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.workbookChartAxisFormat"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartaxisformat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.workbookChartAxisFormat",
  "id": "ded835e6-35e6-ded8-e635-d8dee635d8de"
}
```

