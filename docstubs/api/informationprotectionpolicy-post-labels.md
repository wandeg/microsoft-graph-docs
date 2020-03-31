---
title: "Add labels"
description: "Add labels by posting to the labels collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add labels

Namespace: microsoft.graph

Add labels by posting to the labels collection.

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
POST /informationProtection/policy/labels/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [informationProtectionLabel](../resources/informationprotectionlabel.md) object.

The following table shows the properties that are required when you create the [informationProtectionLabel](../resources/informationprotectionlabel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|description|String||
|color|String||
|sensitivity|Int32||
|tooltip|String||
|isActive|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_informationprotectionlabel_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.informationProtectionLabel",
  "name": "Name value",
  "description": "Description value",
  "color": "Color value",
  "sensitivity": 11,
  "tooltip": "Tooltip value",
  "isActive": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationprotectionlabel"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 282

{
  "@odata.type": "#microsoft.graph.informationProtectionLabel",
  "id": "1457a7e3-a7e3-1457-e3a7-5714e3a75714",
  "name": "Name value",
  "description": "Description value",
  "color": "Color value",
  "sensitivity": 11,
  "tooltip": "Tooltip value",
  "isActive": true
}
```

