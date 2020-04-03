---
title: "Get conditionalAccessPolicy"
description: "Read properties and relationships of the conditionalAccessPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get conditionalAccessPolicy

Namespace: microsoft.graph

Read properties and relationships of the [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.

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
GET /policies/conditionalAccessPolicies/{conditionalAccessPolicyId}
GET /identity/conditionalAccess/policies/{conditionalAccessPolicyId}
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
If successful, this method returns a `200 OK` response code and [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/conditionalAccessPolicies/{conditionalAccessPolicyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3572

{
  "value": {
    "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
    "id": "33ec3667-3667-33ec-6736-ec336736ec33",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "modifiedDateTime": "2016-12-31T23:58:55.6791311+00:00",
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
}
```

