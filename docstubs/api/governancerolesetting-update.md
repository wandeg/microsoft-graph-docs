---
title: "Update governanceRoleSetting"
description: "Update the properties of a governanceRoleSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update governanceRoleSetting

Namespace: microsoft.graph

Update the properties of a [governanceRoleSetting](../resources/governancerolesetting.md) object.

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
PATCH /governanceRoleSettings/{governanceRoleSettingsId}
PATCH /governanceRoleDefinitions/{governanceRoleDefinitionsId}/roleSetting
PATCH /privilegedAccess/{privilegedAccessId}/roleSettings/{governanceRoleSettingId}
PATCH /governanceResources/{governanceResourcesId}/roleSettings/{governanceRoleSettingId}
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleSettings/{governanceRoleSettingId}
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [governanceRoleSetting](../resources/governancerolesetting.md) object.

The following table shows the properties that are required when you create the [governanceRoleSetting](../resources/governancerolesetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceId|String||
|roleDefinitionId|String||
|isDefault|Boolean||
|lastUpdatedDateTime|DateTimeOffset||
|lastUpdatedBy|String||
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceRoleSettings/{governanceRoleSettingsId}
Content-type: application/json
Content-length: 809

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2016-12-31T23:56:44.5564137+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 858

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "9d79344a-344a-9d79-4a34-799d4a34799d",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2016-12-31T23:56:44.5564137+03:00",
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

