---
title: "Create userFlows"
description: "Create a new userFlows object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create userFlows

Namespace: microsoft.cpim.api.dataModels

Create a new userFlows object.

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
POST /identity/userFlows
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object.

The following table shows the properties that are required when you create the [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|userFlowType|userFlowType|**TODO: Add Description**. Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Single|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-Type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityUserFlow",
  "userFlowType": "String",
  "userFlowTypeVersion": "Single"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.datamodels.identityuserflow"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityUserFlow",
  "id": "68824056-4056-6882-5640-826856408268",
  "userFlowType": "String",
  "userFlowTypeVersion": "Single"
}
```

