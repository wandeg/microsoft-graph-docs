---
title: "Update multiValueExtendedProperties"
description: "Update the properties of a multiValueExtendedProperties object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update multiValueExtendedProperties

Namespace: microsoft.graph

Update the properties of a multiValueExtendedProperties object.

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
PATCH /invitations/{invitationsId}/invitedUser/calendar/events/{eventId}/multiValueExtendedProperties
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

The following table shows the properties that are required when you create the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|value|String collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_multivalueextendedproperties"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/calendar/events/{eventId}/multiValueExtendedProperties
Content-Type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "value": [
    "Value value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "id": "a5526718-6718-a552-1867-52a5186752a5",
  "value": [
    "Value value"
  ]
}
```

