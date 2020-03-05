---
title: "List singleValueExtendedProperties"
description: "Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List singleValueExtendedProperties

Namespace: microsoft.graph

Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.

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
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/singleValueExtendedProperties
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages/{messageId}/microsoft.graph.eventMessage/event/singleValueExtendedProperties
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.singlevaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
      "id": "45351890-1890-4535-9018-354590183545",
      "value": "Value value"
    }
  ]
}
```

