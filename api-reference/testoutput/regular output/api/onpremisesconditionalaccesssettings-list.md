---
title: "List onPremisesConditionalAccessSettingses"
description: "List properties and relationships of the onPremisesConditionalAccessSettings objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onPremisesConditionalAccessSettingses

Namespace: microsoft.graph

List properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) objects.

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
GET ** Collection URI for microsoft.graph.onPremisesConditionalAccessSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisesconditionalaccesssettings"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.onPremisesConditionalAccessSettings not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onpremisesconditionalaccesssettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
      "id": "f2ed9cc3-9cc3-f2ed-c39c-edf2c39cedf2",
      "enabled": true,
      "includedGroups": [
        "0d12d1f7-d1f7-0d12-f7d1-120df7d1120d"
      ],
      "excludedGroups": [
        "967dd801-d801-967d-01d8-7d9601d87d96"
      ],
      "overrideDefaultRule": true
    }
  ]
}
```

