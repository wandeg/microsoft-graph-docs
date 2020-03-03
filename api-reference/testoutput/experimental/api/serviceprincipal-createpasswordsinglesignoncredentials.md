---
title: "createPasswordSingleSignOnCredentials"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createPasswordSingleSignOnCredentials

Namespace: microsoft.graph



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
POST /servicePrincipals/{servicePrincipalsId}/createPasswordSingleSignOnCredentials
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|credentials|[credential](../resources/credential.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_createpasswordsinglesignoncredentials"
}
-->
``` http
POST https://graph.microsoft.com/localtest/servicePrincipals/{servicePrincipalsId}/createPasswordSingleSignOnCredentials

Content-type: application/json
Content-length: 115

{
  "id": "Id value",
  "credentials": [
    {
      "@odata.type": "microsoft.graph.credential"
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordsinglesignoncredentialset"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "value": {
    "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet"
  }
}
```

