---
title: "Create credentialUserRegistrationCount"
description: "Create a new credentialUserRegistrationCount object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create credentialUserRegistrationCount

Namespace: microsoft.graph

Create a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object.

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
POST ** Collection URI for microsoft.graph.credentialUserRegistrationCount not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object.

The following table shows the properties that are required when you create the [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|totalUserCount|Int64||
|userRegistrationCounts|[userRegistrationCount](../resources/userregistrationcount.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_credentialuserregistrationcount_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.credentialUserRegistrationCount not found
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
  "totalUserCount": 14,
  "userRegistrationCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationCount",
      "registrationStatus": "String",
      "registrationCount": 1
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialuserregistrationcount"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
  "id": "1bc6be74-be74-1bc6-74be-c61b74bec61b",
  "totalUserCount": 14,
  "userRegistrationCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationCount",
      "registrationStatus": "String",
      "registrationCount": 1
    }
  ]
}
```

