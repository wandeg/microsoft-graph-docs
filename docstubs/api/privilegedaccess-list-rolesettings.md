---
title: "List roleSettings"
description: "Get the governanceRoleSettings from the roleSettings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List roleSettings

Namespace: microsoft.graph

Get the governanceRoleSettings from the roleSettings navigation property.

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
GET /privilegedAccess/{privilegedAccessId}/roleSettings
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}/roleSettings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governancerolesetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1007

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.governanceRoleSetting",
      "id": "2ae8f95e-f95e-2ae8-5ef9-e82a5ef9e82a",
      "resourceId": "Resource Id value",
      "roleDefinitionId": "Role Definition Id value",
      "isDefault": true,
      "lastUpdatedDateTime": "2016-12-31T23:57:43.3634504+03:00",
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
  ]
}
```

