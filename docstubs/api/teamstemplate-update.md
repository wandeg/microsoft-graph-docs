---
title: "Update teamsTemplate"
description: "Update the properties of a teamsTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsTemplate

Namespace: microsoft.graph

Update the properties of a [teamsTemplate](../resources/teamstemplate.md) object.

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
PATCH /teamsTemplates/{teamsTemplatesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [teamsTemplate](../resources/teamstemplate.md) object.

The following table shows the properties that are required when you create the [teamsTemplate](../resources/teamstemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsTemplate](../resources/teamstemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamstemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teamsTemplates/{teamsTemplatesId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.teamsTemplate",
  "id": "17c7f1be-f1be-17c7-bef1-c717bef1c717"
}
```

