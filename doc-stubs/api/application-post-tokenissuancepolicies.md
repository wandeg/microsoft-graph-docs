---
title: "Add tokenIssuancePolicies"
description: "Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add tokenIssuancePolicies
Namespace: microsoft.graph

Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.

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
POST /policies/tokenIssuancePolicies/$ref
POST /applications/{applicationsId}/tokenIssuancePolicies/$ref
POST /servicePrincipals/{servicePrincipalsId}/tokenIssuancePolicies/$ref
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
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|



## Response

If successful, this method returns a `204 No Content` response code and a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/$ref
Content-Type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "deletedDateTime": "String (timestamp)",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenissuancepolicy"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "id": "ae5002ff-02ff-ae50-ff02-50aeff0250ae",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

