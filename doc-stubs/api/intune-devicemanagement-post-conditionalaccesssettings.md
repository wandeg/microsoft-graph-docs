---
title: "Create conditionalAccessSettings"
description: "Create a new conditionalAccessSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create conditionalAccessSettings

Namespace: microsoft.graph

Create a new conditionalAccessSettings object.

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
POST /deviceManagement/conditionalAccessSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onPremisesConditionalAccessSettings](../resources/intune-onpremisesconditionalaccesssettings.md) object.

The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onpremisesconditionalaccesssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|enabled|Boolean|**TODO: Add Description**|
|includedGroups|Guid collection|**TODO: Add Description**|
|excludedGroups|Guid collection|**TODO: Add Description**|
|overrideDefaultRule|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [onPremisesConditionalAccessSettings](../resources/intune-onpremisesconditionalaccesssettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onpremisesconditionalaccesssettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-Type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": "Boolean",
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onpremisesconditionalaccesssettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "9852dc16-dc16-9852-16dc-529816dc5298",
  "enabled": "Boolean",
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": "Boolean"
}
```

