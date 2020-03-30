---
title: "Create teamsTemplate"
description: "Create a new teamsTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsTemplate

Namespace: microsoft.graph

Create a new [teamsTemplate](../resources/teamstemplate.md) object.

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
POST /teamsTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [teamsTemplate](../resources/teamstemplate.md) object.

The following table shows the properties that are required when you create the [teamsTemplate](../resources/teamstemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [teamsTemplate](../resources/teamstemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamstemplate_from_teamstemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamsTemplates
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.teamsTemplate"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamstemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.teamsTemplate",
  "id": "0b415c77-5c77-0b41-775c-410b775c410b"
}
```

