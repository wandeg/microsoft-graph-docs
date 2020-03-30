---
title: "Add featureRolloutPolicies"
description: "Add featureRolloutPolicies by posting to the featureRolloutPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add featureRolloutPolicies

Namespace: microsoft.graph

Add featureRolloutPolicies by posting to the featureRolloutPolicies collection.

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
POST /directory/featureRolloutPolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.

The following table shows the properties that are required when you create the [featureRolloutPolicy](../resources/featurerolloutpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|feature|Enumeration| Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|isEnabled|Boolean||
|isAppliedToOrganization|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featurerolloutpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.featureRolloutPolicy",
  "id": "642dfe6f-fe6f-642d-6ffe-2d646ffe2d64",
  "displayName": "Display Name value",
  "description": "Description value",
  "feature": "String",
  "isEnabled": true,
  "isAppliedToOrganization": true
}
```

