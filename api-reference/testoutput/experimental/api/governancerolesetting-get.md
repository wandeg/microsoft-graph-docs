---
title: "Get governanceRoleSetting"
description: "Read properties and relationships of the governanceRoleSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get governanceRoleSetting

Read properties and relationships of the [governanceRoleSetting](../resources/governancerolesetting.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /governanceRoleSettings/{governanceRoleSettingsId}
GET /governanceRoleDefinitions/{governanceRoleDefinitionsId}/roleSetting
GET /privilegedAccess/{privilegedAccessId}/roleSettings/{governanceRoleSettingId}
GET /governanceResources/{governanceResourcesId}/roleSettings/{governanceRoleSettingId}
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleSettings/{governanceRoleSettingId}
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/governanceRoleSettings/{governanceRoleSettingsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 935

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceRoleSetting",
    "id": "d8950804-0804-d895-0408-95d8040895d8",
    "resourceId": "Resource Id value",
    "roleDefinitionId": "Role Definition Id value",
    "isDefault": true,
    "lastUpdatedDateTime": "2017-01-01T00:01:04.1563754+03:00",
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
}
```

