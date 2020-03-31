---
title: "Add userFlows"
description: "Add userFlows by posting to the userFlows collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userFlows

Namespace: microsoft.graph

Add userFlows by posting to the userFlows collection.

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
POST /identity/userFlows/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [identityUserFlow](../resources/identityuserflow.md) object.

The following table shows the properties that are required when you create the [identityUserFlow](../resources/identityuserflow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userFlowType|Enumeration| Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Single||



## Response
If successful, this method returns a `201 Created` response code and a [identityUserFlow](../resources/identityuserflow.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json
Content-length: 123

{
  "@odata.type": "#microsoft.graph.identityUserFlow",
  "userFlowType": "String",
  "userFlowTypeVersion": "Single"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityuserflow"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 172

{
  "@odata.type": "#microsoft.graph.identityUserFlow",
  "id": "02d2eb8f-eb8f-02d2-8feb-d2028febd202",
  "userFlowType": "String",
  "userFlowTypeVersion": "Single"
}
```

