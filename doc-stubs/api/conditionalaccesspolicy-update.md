---
title: "Update conditionalAccessPolicy"
description: "Update the properties of a conditionalAccessPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update conditionalAccessPolicy
Namespace: microsoft.graph

Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.

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
PATCH /policies/conditionalAccessPolicies/{conditionalAccessPolicyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.

The following table shows the properties that are required when you create the [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|state|conditionalAccessPolicyState|**TODO: Add Description**. Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.|
|conditions|[conditionalAccessConditionSet](../resources/conditionalaccessconditionset.md)|**TODO: Add Description**|
|grantControls|[conditionalAccessGrantControls](../resources/conditionalaccessgrantcontrols.md)|**TODO: Add Description**|
|sessionControls|[conditionalAccessSessionControls](../resources/conditionalaccesssessioncontrols.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/policies/conditionalAccessPolicies/{conditionalAccessPolicyId}
Content-Type: application/json
Content-length: 434

{
  "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
  "displayName": "String",
  "description": "String",
  "state": "String",
  "conditions": {
    "@odata.type": "microsoft.graph.conditionalAccessConditionSet"
  },
  "grantControls": {
    "@odata.type": "microsoft.graph.conditionalAccessGrantControls"
  },
  "sessionControls": {
    "@odata.type": "microsoft.graph.conditionalAccessSessionControls"
  }
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
  "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
  "id": "a171f761-f761-a171-61f7-71a161f771a1",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "state": "String",
  "conditions": {
    "@odata.type": "microsoft.graph.conditionalAccessConditionSet"
  },
  "grantControls": {
    "@odata.type": "microsoft.graph.conditionalAccessGrantControls"
  },
  "sessionControls": {
    "@odata.type": "microsoft.graph.conditionalAccessSessionControls"
  }
}
```

