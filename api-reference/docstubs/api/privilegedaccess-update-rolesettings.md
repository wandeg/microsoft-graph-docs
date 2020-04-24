---
title: "Update roleSettings"
description: "Update the properties of a roleSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update roleSettings

Namespace: microsoft.graph

Update the properties of a roleSettings object.

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
PATCH /privilegedAccess/{privilegedAccessId}/roleSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
  "name": "update_rolesettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}/roleSettings
Content-Type: application/json
Content-length: 809

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
  "lastUpdatedBy": "Last Updated By value",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting",
      "ruleIdentifier": "Rule Identifier value",
      "setting": "Setting value"
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
  "id": "3a7a4fb3-4fb3-3a7a-b34f-7a3ab34f7a3a",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
  "lastUpdatedBy": "Last Updated By value",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting",
      "ruleIdentifier": "Rule Identifier value",
      "setting": "Setting value"
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

