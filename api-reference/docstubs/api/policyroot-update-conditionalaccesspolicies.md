---
title: "Update conditionalAccessPolicies"
description: "Update the properties of a conditionalAccessPolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update conditionalAccessPolicies

Namespace: microsoft.graph

Update the properties of a conditionalAccessPolicies object.

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
PATCH /policies/conditionalAccessPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
  "name": "update_conditionalaccesspolicies"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/conditionalAccessPolicies
Content-Type: application/json
Content-length: 3149

{
  "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
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
```

