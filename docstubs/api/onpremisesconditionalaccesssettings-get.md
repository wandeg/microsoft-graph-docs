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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisesconditionalaccesssettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "c69f2ced-2ced-c69f-ed2c-9fc6ed2c9fc6",
    "enabled": true,
    "includedGroups": [
      "03779923-9923-0377-2399-770323997703"
    ],
    "excludedGroups": [
      "7dc3bac7-bac7-7dc3-c7ba-c37dc7bac37d"
    ],
    "overrideDefaultRule": true
  }
}
```

