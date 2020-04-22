---
title: "Update conditionalAccessSettings"
description: "Update the properties of a conditionalAccessSettings object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update conditionalAccessSettings

Namespace: microsoft.graph

Update the properties of a conditionalAccessSettings object.

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
PATCH /deviceManagement/conditionalAccessSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|enabled|Boolean|Indicates if on premises conditional access is enabled for this organization|
|includedGroups|Guid collection|User groups that will be targeted by on premises conditional access. All users in these groups will be required to have mobile device managed and compliant for mail access.|
|excludedGroups|Guid collection|User groups that will be exempt by on premises conditional access. All users in these groups will be exempt from the conditional access policy.|
|overrideDefaultRule|Boolean|Override the default access rule when allowing a device to ensure access is granted.|



## Response
If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-Type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "522085d7-85d7-5220-d785-2052d7852052"
  ],
  "excludedGroups": [
    "0bda4c9c-4c9c-0bda-9c4c-da0b9c4cda0b"
  ],
  "overrideDefaultRule": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

