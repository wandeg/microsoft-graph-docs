---
title: "Create governanceSubject"
description: "Create a new governanceSubject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create governanceSubject

Namespace: microsoft.graph

Create a new [governanceSubject](../resources/governancesubject.md) object.

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
POST /governanceSubjects
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [governanceSubject](../resources/governancesubject.md) object.

The following table shows the properties that are required when you create the [governanceSubject](../resources/governancesubject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||
|displayName|String||
|principalName|String||
|email|String||



## Response
If successful, this method returns a `201 Created` response code and a [governanceSubject](../resources/governancesubject.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_governancesubject_from_governancesubjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceSubjects
Content-type: application/json
Content-length: 195

{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "type": "Type value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governancesubject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 244

{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "id": "199178f8-78f8-1991-f878-9119f8789119",
  "type": "Type value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value"
}
```

