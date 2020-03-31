---
title: "Update sensitivityPolicySettings"
description: "Update the properties of a sensitivityPolicySettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sensitivityPolicySettings

Namespace: microsoft.graph

Update the properties of a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.

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
PATCH /informationProtection/sensitivityPolicySettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.

The following table shows the properties that are required when you create the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isMandatory|Boolean||
|helpWebUrl|String||
|downgradeSensitivityRequiresJustification|Boolean||
|applicableTo|Enumeration| Possible values are: `email`, `site`, `unifiedGroup`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sensitivitypolicysettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/informationProtection/sensitivityPolicySettings
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.sensitivityPolicySettings",
  "isMandatory": true,
  "helpWebUrl": "https://example.com/helpWebUrl/",
  "downgradeSensitivityRequiresJustification": true,
  "applicableTo": "String"
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
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.sensitivityPolicySettings",
  "id": "2b362131-2131-2b36-3121-362b3121362b",
  "isMandatory": true,
  "helpWebUrl": "https://example.com/helpWebUrl/",
  "downgradeSensitivityRequiresJustification": true,
  "applicableTo": "String"
}
```

