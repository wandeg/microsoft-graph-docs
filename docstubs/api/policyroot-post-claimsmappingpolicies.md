---
title: "Add claimsMappingPolicies"
description: "Add claimsMappingPolicies by posting to the claimsMappingPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add claimsMappingPolicies

Namespace: microsoft.graph

Add claimsMappingPolicies by posting to the claimsMappingPolicies collection.

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
POST /policies/claimsMappingPolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.

The following table shows the properties that are required when you create the [claimsMappingPolicy](../resources/claimsmappingpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|definition|String collection| Inherited from [stsPolicy](../resources/stspolicy.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stspolicy.md)|



## Response
If successful, this method returns a `201 Created` response code and a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.claimsMappingPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsmappingpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.claimsMappingPolicy",
  "id": "30cd61c7-61c7-30cd-c761-cd30c761cd30",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

