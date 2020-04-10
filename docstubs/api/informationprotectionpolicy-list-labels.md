---
title: "List labels"
description: "Get the informationProtectionLabels from the labels navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List labels

Namespace: microsoft.graph

Get the informationProtectionLabels from the labels navigation property.

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
GET /informationProtection/policy/labels
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/policy/labels
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.informationprotectionlabel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.informationProtectionLabel",
      "id": "90835858-5858-9083-5858-839058588390",
      "name": "Name value",
      "description": "Description value",
      "color": "Color value",
      "sensitivity": 11,
      "tooltip": "Tooltip value",
      "isActive": true
    }
  ]
}
```

