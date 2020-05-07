---
title: "Update governanceRoleSetting"
description: "Update the properties of a governanceRoleSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update governanceRoleSetting

Namespace: microsoft.graph

Update the properties of a [governanceRoleSetting](../resources/governancerolesetting.md) object.

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
PATCH /governanceRoleSettings/{governanceRoleSettingsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [governanceRoleSetting](../resources/governancerolesetting.md) object.

The following table shows the properties that are required when you create the [governanceRoleSetting](../resources/governancerolesetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastUpdatedBy|String|**TODO: Add Description**|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceRoleSettings/{governanceRoleSettingsId}
Content-Type: application/json
Content-length: 670

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": "Boolean",
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "adminMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ]
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
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "93e442fc-42fc-93e4-fc42-e493fc42e493",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": "Boolean",
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "adminMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ]
}
```

