---
title: "Create agreementAcceptances"
description: "Create agreementAcceptances by posting to the agreementAcceptances collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create agreementAcceptances

Namespace: microsoft.graph

Create agreementAcceptances by posting to the agreementAcceptances collection.

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
POST /me/agreementAcceptances/$ref
POST /users/{usersId}/agreementAcceptances/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [agreementAcceptance](../resources/agreementacceptance.md) object.

The following table shows the properties that are required when you create the [agreementAcceptance](../resources/agreementacceptance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|agreementId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|agreementFileId|String|**TODO: Add Description**|
|recordedDateTime|DateTimeOffset|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userEmail|String|**TODO: Add Description**|
|state|agreementAcceptanceState|**TODO: Add Description**. Possible values are: `accepted`, `declined`.|



## Response
If successful, this method returns a `201 Created` response code and an [agreementAcceptance](../resources/agreementacceptance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_agreementacceptance_from_agreementacceptances"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/agreementAcceptances
Content-Type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:59:13.0641961+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementacceptance"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "id": "d43afb91-fb91-d43a-91fb-3ad491fb3ad4",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:59:13.0641961+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

