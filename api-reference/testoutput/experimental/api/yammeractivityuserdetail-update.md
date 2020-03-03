---
title: "Update yammerActivityUserDetail"
description: "Update the properties of a yammerActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update yammerActivityUserDetail

Update the properties of a [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.yammerActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [yammerActivityUserDetail](../resources/yammerActivityUserDetail.md) object.

The following table shows the properties that are required when you create the [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|userState|String||
|stateChangeDate|Date||
|lastActivityDate|Date||
|postedCount|Int64||
|readCount|Int64||
|likedCount|Int64||
|assignedProducts|String collection||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_yammeractivityuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.yammerActivityUserDetail not found
Content-type: application/json
Content-length: 454

{
  "@odata.type": "#microsoft.graph.yammerActivityUserDetail",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "userState": "User State value",
  "stateChangeDate": "Date",
  "lastActivityDate": "Date",
  "postedCount": 11,
  "readCount": 9,
  "likedCount": 10,
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

{
  "@odata.type": "#microsoft.graph.yammerActivityUserDetail",
  "id": "f3152655-2655-f315-5526-15f3552615f3",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "userState": "User State value",
  "stateChangeDate": "Date",
  "lastActivityDate": "Date",
  "postedCount": 11,
  "readCount": 9,
  "likedCount": 10,
  "assignedProducts": [
    "Assigned Products value"
  ],
  "reportPeriod": "Report Period value"
}
```

