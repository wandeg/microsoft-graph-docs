---
title: "Create governanceRoleSetting"
description: "Create a new governanceRoleSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create governanceRoleSetting

Namespace: microsoft.graph

Create a new [governanceRoleSetting](../resources/governancerolesetting.md) object.

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
POST /governanceRoleSettings
POST /privilegedAccess/{privilegedAccessId}/roleSettings
POST /governanceResources/{governanceResourcesId}/roleSettings
POST /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_governancerolesetting_from_governancerolesettings"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleSettings
Content-type: application/json
Content-length: 809

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2016-12-31T23:59:36.3019675+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.governancerolesetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 858

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "3bcc8f54-8f54-3bcc-548f-cc3b548fcc3b",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2016-12-31T23:59:36.3019675+00:00",
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

