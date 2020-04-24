---
title: "Create featureRolloutPolicies"
description: "Create a new featureRolloutPolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create featureRolloutPolicies

Namespace: microsoft.graph

Create a new featureRolloutPolicies object.

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
POST /directory/featureRolloutPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.

The following table shows the properties that are required when you create the [featureRolloutPolicy](../resources/featurerolloutpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|feature|stagedFeatureName|**TODO: Add Description**. Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|isEnabled|Boolean|**TODO: Add Description**|
|isAppliedToOrganization|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies
Content-Type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.featureRolloutPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "feature": "String",
  "isEnabled": true,
  "isAppliedToOrganization": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featurerolloutpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.featureRolloutPolicy",
  "id": "11eef388-f388-11ee-88f3-ee1188f3ee11",
  "displayName": "Display Name value",
  "description": "Description value",
  "feature": "String",
  "isEnabled": true,
  "isAppliedToOrganization": true
}
```

