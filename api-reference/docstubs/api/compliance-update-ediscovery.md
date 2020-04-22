---
title: "Update ediscovery"
description: "Update the properties of an ediscovery object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update ediscovery

Namespace: microsoft.graph

Update the properties of an ediscovery object.

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
PATCH /compliance/ediscovery
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [ediscovery](../resources/ediscovery.md) object.

The following table shows the properties that are required when you create the [ediscovery](../resources/ediscovery.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [ediscovery](../resources/ediscovery.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_ediscovery"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery
Content-Type: application/json
Content-length: 52

{
  "@odata.type": "#microsoft.graph.ediscovery"
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
  "@odata.type": "#microsoft.graph.ediscovery",
  "id": "9286da7d-da7d-9286-7dda-86927dda8692"
}
```

