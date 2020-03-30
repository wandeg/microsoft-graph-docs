---
title: "Add roleSettings"
description: "Add roleSettings by posting to the roleSettings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add roleSettings

Namespace: microsoft.graph

Add roleSettings by posting to the roleSettings collection.

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
POST /privilegedAccess/{privilegedAccessId}/roleSettings/$ref
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
POST https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}/roleSettings
Content-type: application/json
Content-length: 808

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2017-01-01T00:01:50.447451+00:00",
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
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "26809dac-9dac-2680-ac9d-8026ac9d8026",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "isDefault": true,
  "lastUpdatedDateTime": "2017-01-01T00:01:50.447451+00:00",
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

