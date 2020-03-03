---
title: "Update aadUserConversationMember"
description: "Update the properties of a aadUserConversationMember object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update aadUserConversationMember

Update the properties of a [aadUserConversationMember](../resources/aaduserconversationmember.md) object.

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
PATCH ** Entity URI for microsoft.graph.aadUserConversationMember not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [aadUserConversationMember](../resources/aadUserConversationMember.md) object.

The following table shows the properties that are required when you create the [aadUserConversationMember](../resources/aaduserconversationmember.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|roles|String collection| Inherited from [conversationMember](../resources/conversationMember.md)|
|displayName|String| Inherited from [conversationMember](../resources/conversationMember.md)|
|userId|String||
|email|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [aadUserConversationMember](../resources/aaduserconversationmember.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_aaduserconversationmember"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.aadUserConversationMember not found
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [
    "Roles value"
  ],
  "displayName": "Display Name value",
  "userId": "User Id value",
  "email": "Email value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "928ebc1f-bc1f-928e-1fbc-8e921fbc8e92",
  "roles": [
    "Roles value"
  ],
  "displayName": "Display Name value",
  "userId": "User Id value",
  "email": "Email value"
}
```

