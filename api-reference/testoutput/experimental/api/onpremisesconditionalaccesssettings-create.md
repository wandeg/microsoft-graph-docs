---
title: "Create onPremisesConditionalAccessSettings"
description: "Create a new onPremisesConditionalAccessSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create onPremisesConditionalAccessSettings

Namespace: microsoft.graph

Create a new [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

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
POST ** Collection URI for microsoft.graph.onPremisesConditionalAccessSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|enabled|Boolean|Indicates if on premises conditional access is enabled for this organization|
|includedGroups|Guid collection|User groups that will be targeted by on premises conditional access. All users in these groups will be required to have mobile device managed and compliant for mail access.|
|excludedGroups|Guid collection|User groups that will be exempt by on premises conditional access. All users in these groups will be exempt from the conditional access policy.|
|overrideDefaultRule|Boolean|Override the default access rule when allowing a device to ensure access is granted.|



## Response
If successful, this method returns a `201 Created` response code and a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onpremisesconditionalaccesssettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.onPremisesConditionalAccessSettings not found
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "812dbfa7-bfa7-812d-a7bf-2d81a7bf2d81"
  ],
  "excludedGroups": [
    "c03641ed-41ed-c036-ed41-36c0ed4136c0"
  ],
  "overrideDefaultRule": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onpremisesconditionalaccesssettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "ce6b7a76-7a76-ce6b-767a-6bce767a6bce",
  "enabled": true,
  "includedGroups": [
    "812dbfa7-bfa7-812d-a7bf-2d81a7bf2d81"
  ],
  "excludedGroups": [
    "c03641ed-41ed-c036-ed41-36c0ed4136c0"
  ],
  "overrideDefaultRule": true
}
```

