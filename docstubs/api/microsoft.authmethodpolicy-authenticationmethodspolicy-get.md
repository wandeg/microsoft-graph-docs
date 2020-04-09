---
title: "Get authenticationMethodsPolicy"
description: "Read properties and relationships of the authenticationMethodsPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get authenticationMethodsPolicy

Namespace: microsoft.authMethodPolicy

Read properties and relationships of the [authenticationMethodsPolicy](../resources/microsoft.authmethodpolicy-authenticationmethodspolicy.md) object.

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
GET /authenticationMethodsPolicy
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
If successful, this method returns a `200 OK` response code and [authenticationMethodsPolicy](../resources/microsoft.authmethodpolicy-authenticationmethodspolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/authenticationMethodsPolicy
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.authMethodPolicy.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 940

{
  "value": {
    "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodsPolicy",
    "id": "4a8f8c7d-8c7d-4a8f-7d8c-8f4a7d8c8f4a",
    "displayName": "Display Name value",
    "description": "Description value",
    "lastModifiedDateTime": "2016-12-31T23:57:48.7572956+03:00",
    "policyVersion": "Policy Version value",
    "convergedPolicyTargetGroup": "Converged Policy Target Group value",
    "registrationAndResetTargets": [
      {
        "@odata.type": "microsoft.authMethodPolicy.registrationAndResetTarget",
        "targetType": "String",
        "id": "Id value",
        "minAuthMethodsToRegister": 8,
        "minAuthMethodsToReset": 5
      }
    ],
    "registrationEnforcement": {
      "@odata.type": "microsoft.authMethodPolicy.registrationEnforcement",
      "isAllowedToSkipRegistration": true,
      "registrationSkipDurationInDays": 14
    },
    "reconfirmationInDays": 4
  }
}
```

