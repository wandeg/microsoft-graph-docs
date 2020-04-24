---
title: "List policies"
description: "Get the conditionalAccessPolicies from the policies navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List policies

Namespace: microsoft.graph

Get the conditionalAccessPolicies from the policies navigation property.

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
GET /identity/conditionalAccess/policies
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.conditionalaccesspolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
      "id": "888162b2-62b2-8881-b262-8188b2628188",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "state": "String",
      "conditions": {
        "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
        "applications": {
          "@odata.type": "microsoft.graph.conditionalAccessApplications",
          "includeApplications": [
            "Include Applications value"
          ],
          "excludeApplications": [
            "Exclude Applications value"
          ],
          "includeUserActions": [
            "Include User Actions value"
          ]
        },
        "users": {
          "@odata.type": "microsoft.graph.conditionalAccessUsers",
          "includeUsers": [
            "Include Users value"
          ],
          "excludeUsers": [
            "Exclude Users value"
          ],
          "includeGroups": [
            "Include Groups value"
          ],
          "excludeGroups": [
            "Exclude Groups value"
          ],
          "includeRoles": [
            "Include Roles value"
          ],
          "excludeRoles": [
            "Exclude Roles value"
          ]
        },
        "signInRiskLevels": [
          "String"
        ],
        "platforms": {
          "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
          "includePlatforms": [
            "String"
          ],
          "excludePlatforms": [
            "String"
          ]
        },
        "locations": {
          "@odata.type": "microsoft.graph.conditionalAccessLocations",
          "includeLocations": [
            "Include Locations value"
          ],
          "excludeLocations": [
            "Exclude Locations value"
          ]
        },
        "clientAppTypes": [
          "String"
        ],
        "deviceStates": {
          "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
          "includeStates": [
            "Include States value"
          ],
          "excludeStates": [
            "Exclude States value"
          ]
        },
        "devices": {
          "@odata.type": "microsoft.graph.conditionalAccessDevices",
          "includeDeviceStates": [
            "Include Device States value"
          ],
          "excludeDeviceStates": [
            "Exclude Device States value"
          ]
        }
      },
      "grantControls": {
        "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
        "operator": "Operator value",
        "builtInControls": [
          "String"
        ],
        "customAuthenticationFactors": [
          "Custom Authentication Factors value"
        ],
        "termsOfUse": [
          "Terms Of Use value"
        ]
      },
      "sessionControls": {
        "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
        "applicationEnforcedRestrictions": {
          "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
          "isEnabled": true
        },
        "cloudAppSecurity": {
          "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
          "cloudAppSecurityType": "String"
        },
        "signInFrequency": {
          "@odata.type": "microsoft.graph.signInFrequencySessionControl",
          "value": 5,
          "type": "String"
        },
        "persistentBrowser": {
          "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
          "mode": "String"
        }
      }
    }
  ]
}
```

