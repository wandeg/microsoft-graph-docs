---
title: "List conditionalAccessSettings"
description: "Get the onPremisesConditionalAccessSettings from the conditionalAccessSettings navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List conditionalAccessSettings

Namespace: microsoft.graph

Get the onPremisesConditionalAccessSettings from the conditionalAccessSettings navigation property.

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
GET /deviceManagement/conditionalAccessSettings
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) objects in the response body.

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
  "@odata.type": "collection(microsoft.graph.onpremisesconditionalaccesssettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
      "id": "117bfdef-fdef-117b-effd-7b11effd7b11",
      "enabled": true,
      "includedGroups": [
        "522085d7-85d7-5220-d785-2052d7852052"
      ],
      "excludedGroups": [
        "0bda4c9c-4c9c-0bda-9c4c-da0b9c4cda0b"
      ],
      "overrideDefaultRule": true
    }
  ]
}
```

