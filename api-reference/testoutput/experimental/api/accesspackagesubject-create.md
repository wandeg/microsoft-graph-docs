---
title: "Create accessPackageSubject"
description: "Create a new accessPackageSubject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackageSubject

Namespace: microsoft.graph

Create a new [accessPackageSubject](../resources/accesspackagesubject.md) object.

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
POST ** Collection URI for microsoft.graph.accessPackageSubject not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [accessPackageSubject](../resources/accesspackagesubject.md) object.

The following table shows the properties that are required when you create the [accessPackageSubject](../resources/accesspackagesubject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|objectId|String||
|altSecId|String||
|displayName|String||
|principalName|String||
|email|String||
|onPremisesSecurityIdentifier|String||
|type|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageSubject](../resources/accesspackagesubject.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackagesubject_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.accessPackageSubject not found
Content-type: application/json
Content-length: 343

{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "objectId": "Object Id value",
  "altSecId": "Alt Sec Id value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "type": "Type value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackagesubject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 392

{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "a24dca23-ca23-a24d-23ca-4da223ca4da2",
  "objectId": "Object Id value",
  "altSecId": "Alt Sec Id value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "type": "Type value"
}
```

