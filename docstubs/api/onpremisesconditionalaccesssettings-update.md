---
title: "Update onPremisesConditionalAccessSettings"
description: "Update the properties of a onPremisesConditionalAccessSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onPremisesConditionalAccessSettings

Namespace: microsoft.graph

Update the properties of a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

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
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|enabled|Boolean||
|includedGroups|Guid collection||
|excludedGroups|Guid collection||
|overrideDefaultRule|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onpremisesconditionalaccesssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "54296f71-6f71-5429-716f-2954716f2954"
  ],
  "excludedGroups": [
    "cc190eb9-0eb9-cc19-b90e-19ccb90e19cc"
  ],
  "overrideDefaultRule": true
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
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "fc1cc67e-c67e-fc1c-7ec6-1cfc7ec61cfc",
  "enabled": true,
  "includedGroups": [
    "54296f71-6f71-5429-716f-2954716f2954"
  ],
  "excludedGroups": [
    "cc190eb9-0eb9-cc19-b90e-19ccb90e19cc"
  ],
  "overrideDefaultRule": true
}
```

