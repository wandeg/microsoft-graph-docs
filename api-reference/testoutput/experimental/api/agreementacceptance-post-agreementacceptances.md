---
title: "Create agreementAcceptance"
description: "Create a new agreementAcceptance object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create agreementAcceptance

Namespace: microsoft.graph

Create a new [agreementAcceptance](../resources/agreementacceptance.md) object.

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
POST /agreementAcceptances
```

## Request headers
|Header|Value|
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
|state|Enumeration|. Possible values are: `accepted`, `declined`.|



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
POST https://graph.microsoft.com/localtest/agreementAcceptances
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2017-01-01T00:02:46.1967034+03:00",
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
  "id": "6b1a007a-007a-6b1a-7a00-1a6b7a001a6b",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2017-01-01T00:02:46.1967034+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

