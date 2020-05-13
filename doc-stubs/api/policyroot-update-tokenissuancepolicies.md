---
title: "Update tokenIssuancePolicies"
description: "Update the properties of a tokenIssuancePolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update tokenIssuancePolicies

Namespace: microsoft.graph

Update the properties of a tokenIssuancePolicies object.

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
PATCH /policies/tokenIssuancePolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.

The following table shows the properties that are required when you create the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicies"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
Content-Type: application/json
Content-length: 195

{
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
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
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "id": "c0dc0485-0485-c0dc-8504-dcc08504dcc0",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

