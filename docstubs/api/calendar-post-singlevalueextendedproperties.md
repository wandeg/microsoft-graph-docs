---
title: "Add singleValueExtendedProperties"
description: "Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add singleValueExtendedProperties

Namespace: microsoft.graph

Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.

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
POST /me/messages/{messageId}/event/calendar/singleValueExtendedProperties/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.

The following table shows the properties that are required when you create the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|value|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_singlevaluelegacyextendedproperty_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/messages/{messageId}/event/calendar/singleValueExtendedProperties
Content-Type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
  "value": "Value value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.singlevaluelegacyextendedproperty"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
  "id": "dff3ec9a-ec9a-dff3-9aec-f3df9aecf3df",
  "value": "Value value"
}
```

