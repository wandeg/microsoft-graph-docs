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

## HTTP request
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

## Examples

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
      "id": "9dec78cf-78cf-9dec-cf78-ec9dcf78ec9d",
      "enabled": true,
      "includedGroups": [
        "6f75ec9e-ec9e-6f75-9eec-756f9eec756f"
      ],
      "excludedGroups": [
        "2dcf6cbc-6cbc-2dcf-bc6c-cf2dbc6ccf2d"
      ],
      "overrideDefaultRule": true
    }
  ]
}
```

