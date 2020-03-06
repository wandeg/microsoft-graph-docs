---
title: "Update featureRolloutPolicy"
description: "Update the properties of a featureRolloutPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update featureRolloutPolicy

Namespace: microsoft.graph

Update the properties of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.

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
PATCH /directory/featureRolloutPolicies/{featureRolloutPolicyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.

The following table shows the properties that are required when you create the [featureRolloutPolicy](../resources/featurerolloutpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|feature|Enumeration|. Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|isEnabled|Boolean||
|isAppliedToOrganization|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/directory/featureRolloutPolicies/{featureRolloutPolicyId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.featureRolloutPolicy",
  "id": "e51902b8-02b8-e519-b802-19e5b80219e5",
  "displayName": "Display Name value",
  "description": "Description value",
  "feature": "String",
  "isEnabled": true,
  "isAppliedToOrganization": true
}
```

