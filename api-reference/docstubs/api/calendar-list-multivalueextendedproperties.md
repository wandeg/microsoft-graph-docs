---
title: "List multiValueExtendedProperties"
description: "Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List multiValueExtendedProperties

Namespace: microsoft.graph

Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.

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
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/event/calendar/multiValueExtendedProperties
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
If successful, this method returns a `200 OK` response code and a collection of [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_multivaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/messages/{messageId}/event/calendar/multiValueExtendedProperties
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.multivaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
      "id": "c25d6eea-6eea-c25d-ea6e-5dc2ea6e5dc2",
      "value": [
        "Value value"
      ]
    }
  ]
}
```

