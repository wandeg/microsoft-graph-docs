---
title: "Create businessFlowTemplate"
description: "Create a new businessFlowTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create businessFlowTemplate

Namespace: microsoft.graph

Create a new [businessFlowTemplate](../resources/businessflowtemplate.md) object.

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
POST /businessFlowTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [businessFlowTemplate](../resources/businessflowtemplate.md) object.

The following table shows the properties that are required when you create the [businessFlowTemplate](../resources/businessflowtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [businessFlowTemplate](../resources/businessflowtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_businessflowtemplate_from_businessflowtemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/businessFlowTemplates
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.businessFlowTemplate",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessflowtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.businessFlowTemplate",
  "id": "df3b664f-664f-df3b-4f66-3bdf4f663bdf",
  "displayName": "Display Name value"
}
```

