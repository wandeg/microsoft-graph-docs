---
title: "Update itemActivity"
description: "Update the properties of a itemActivity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update itemActivity

Namespace: microsoft.graph

Update the properties of a [itemActivity](../resources/itemactivity.md) object.

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
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [itemActivity](../resources/itemactivity.md) object.

The following table shows the properties that are required when you create the [itemActivity](../resources/itemactivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|access|[accessAction](../resources/accessaction.md)||
|activityDateTime|DateTimeOffset||
|actor|[identitySet](../resources/identityset.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [itemActivity](../resources/itemactivity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_itemactivity"
}
-->
``` http

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
Content-Length: 599

{
  "@odata.type": "#microsoft.graph.itemActivity",
  "id": "7ac90dad-0dad-7ac9-ad0d-c97aad0dc97a",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "2016-12-31T23:58:36.9952608+00:00",
  "actor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

