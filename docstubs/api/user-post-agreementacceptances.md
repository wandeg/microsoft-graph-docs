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
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
|state|Enumeration| Possible values are: `accepted`, `declined`.|



## Response
If successful, this method returns a `201 Created` response code and a [agreementAcceptance](../resources/agreementacceptance.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_agreementacceptance_from_agreementacceptances"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/agreementAcceptances
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:58:38.4419584+00:00",
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
  "id": "b04177e8-77e8-b041-e877-41b0e87741b0",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:58:38.4419584+00:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

