---
title: "Create allowedUsers"
description: "Create allowedUsers by posting to the allowedUsers collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create allowedUsers

Namespace: microsoft.graph

Create allowedUsers by posting to the allowedUsers collection.

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
POST /print/printers/{printerId}/allowedUsers/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [printUserIdentity](../resources/printuseridentity.md) object.

The following table shows the properties that are required when you create the [printUserIdentity](../resources/printuseridentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|ipAddress|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `201 Created` response code and a [printUserIdentity](../resources/printuseridentity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printuseridentity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/allowedUsers
Content-type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "displayName": "Display Name value",
  "ipAddress": "Ip Address value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printuseridentity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "id": "9bb114a0-14a0-9bb1-a014-b19ba014b19b",
  "displayName": "Display Name value",
  "ipAddress": "Ip Address value",
  "userPrincipalName": "User Principal Name value"
}
```

