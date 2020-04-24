---
title: "Update informationProtectionLabel"
description: "Update the properties of an informationProtectionLabel object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update informationProtectionLabel

Namespace: microsoft.graph

Update the properties of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.

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
PATCH /invitations/{invitationsId}/invitedUser/informationProtection/policy/labels/{informationProtectionLabelId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [informationProtectionLabel](../resources/informationprotectionlabel.md) object.

The following table shows the properties that are required when you create the [informationProtectionLabel](../resources/informationprotectionlabel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|color|String|**TODO: Add Description**|
|sensitivity|Int32|**TODO: Add Description**|
|tooltip|String|**TODO: Add Description**|
|isActive|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_informationprotectionlabel"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/informationProtection/policy/labels/{informationProtectionLabelId}
Content-Type: application/json
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
  "@odata.type": "#microsoft.graph.informationProtectionLabel",
  "id": "9233d9be-d9be-9233-bed9-3392bed93392",
  "name": "Name value",
  "description": "Description value",
  "color": "Color value",
  "sensitivity": 11,
  "tooltip": "Tooltip value",
  "isActive": true
}
```

