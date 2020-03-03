---
title: "Create agreementAcceptances"
description: "Create agreementAcceptances by posting to the agreementAcceptances collection."
author: ""
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
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/agreementAcceptances/$ref
POST /users/{usersId}/agreementAcceptances/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [agreementAcceptance](../resources/agreementacceptance.md) object.

The following table shows the properties that are required when you create the [agreementAcceptance](../resources/agreementacceptance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|agreementId|String||
|userId|String||
|agreementFileId|String||
|recordedDateTime|DateTimeOffset||
|userDisplayName|String||
|userPrincipalName|String||
|userEmail|String||
|state|Enumeration|. Possible values are: `accepted`, `declined`.|



## Response
If successful, this method returns a `201 Created` response code and a [agreementAcceptance](../resources/agreementacceptance.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_agreementacceptance_from_agreementacceptances"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/agreementAcceptances
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:56:27.4887157+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementacceptance"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 449

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "id": "2b6dc9c2-c9c2-2b6d-c2c9-6d2bc2c96d2b",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:56:27.4887157+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

