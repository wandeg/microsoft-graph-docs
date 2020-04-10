---
title: "Get onPremisesConditionalAccessSettings"
description: "Read properties and relationships of the onPremisesConditionalAccessSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onPremisesConditionalAccessSettings

Namespace: microsoft.graph

Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

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
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
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
If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onpremisesconditionalaccesssettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "1124bec1-bec1-1124-c1be-2411c1be2411",
    "enabled": true,
    "includedGroups": [
      "a9802db3-2db3-a980-b32d-80a9b32d80a9"
    ],
    "excludedGroups": [
      "0acb1666-1666-0acb-6616-cb0a6616cb0a"
    ],
    "overrideDefaultRule": true
  }
}
```

