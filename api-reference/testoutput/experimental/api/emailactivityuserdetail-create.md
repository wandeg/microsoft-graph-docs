---
title: "Create emailActivityUserDetail"
description: "Create a new emailActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create emailActivityUserDetail

Namespace: microsoft.graph

Create a new [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object.

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
POST ** Collection URI for microsoft.graph.emailActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object.

The following table shows the properties that are required when you create the [emailActivityUserDetail](../resources/emailactivityuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|isDeleted|Boolean||
|deletedDate|Date||
|lastActivityDate|Date||
|sendCount|Int64||
|receiveCount|Int64||
|readCount|Int64||
|assignedProducts|String collection||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_emailactivityuserdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.emailActivityUserDetail not found
Content-type: application/json
Content-length: 434

{
  "@odata.type": "#microsoft.graph.emailActivityUserDetail",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "sendCount": 9,
  "receiveCount": 12,
  "readCount": 9,
  "assignedProducts": [
    "Assigned Products value"
  ],
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailactivityuserdetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.emailActivityUserDetail",
  "id": "aa341e5f-1e5f-aa34-5f1e-34aa5f1e34aa",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "sendCount": 9,
  "receiveCount": 12,
  "readCount": 9,
  "assignedProducts": [
    "Assigned Products value"
  ],
  "reportPeriod": "Report Period value"
}
```

