---
title: "Create sensitivityPolicySettings"
description: "Create a new sensitivityPolicySettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create sensitivityPolicySettings

Namespace: microsoft.graph

Create a new sensitivityPolicySettings object.

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
POST /users/{usersId}/informationProtection/sensitivityPolicySettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.

The following table shows the properties that are required when you create the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isMandatory|Boolean|**TODO: Add Description**|
|helpWebUrl|String|**TODO: Add Description**|
|downgradeSensitivityRequiresJustification|Boolean|**TODO: Add Description**|
|applicableTo|sensitivityLabelTarget|**TODO: Add Description**. Possible values are: `email`, `site`, `unifiedGroup`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_sensitivitypolicysettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/informationProtection/sensitivityPolicySettings
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.sensitivityPolicySettings",
  "isMandatory": "Boolean",
  "helpWebUrl": "String",
  "downgradeSensitivityRequiresJustification": "Boolean",
  "applicableTo": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivitypolicysettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.sensitivityPolicySettings",
  "id": "ee4f0dd4-0dd4-ee4f-d40d-4feed40d4fee",
  "isMandatory": "Boolean",
  "helpWebUrl": "String",
  "downgradeSensitivityRequiresJustification": "Boolean",
  "applicableTo": "String"
}
```

