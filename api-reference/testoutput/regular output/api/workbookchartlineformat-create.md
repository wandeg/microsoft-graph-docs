---
title: "Create workbookChartLineFormat"
description: "Create a new workbookChartLineFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartLineFormat

Namespace: microsoft.graph

Create a new [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartLineFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.

The following table shows the properties that are required when you create the [workbookChartLineFormat](../resources/workbookchartlineformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|color|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartlineformat_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartLineFormat not found
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.workbookChartLineFormat",
  "color": "Color value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartlineformat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 141

{
  "@odata.type": "#microsoft.graph.workbookChartLineFormat",
  "id": "659ca35e-a35e-659c-5ea3-9c655ea39c65",
  "color": "Color value"
}
```

