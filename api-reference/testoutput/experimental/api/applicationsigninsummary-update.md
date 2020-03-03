---
title: "Update applicationSignInSummary"
description: "Update the properties of a applicationSignInSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update applicationSignInSummary

Update the properties of a [applicationSignInSummary](../resources/applicationsigninsummary.md) object.

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
PATCH ** Entity URI for microsoft.graph.applicationSignInSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [applicationSignInSummary](../resources/applicationSignInSummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInSummary](../resources/applicationsigninsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appDisplayName|String||
|successfulSignInCount|Int64||
|failedSignInCount|Int64||
|successPercentage|Double||



## Response
If successful, this method returns a `200 OK` response code and an updated [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_applicationsigninsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.applicationSignInSummary not found
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "appDisplayName": "App Display Name value",
  "successfulSignInCount": 5,
  "failedSignInCount": 1,
  "successPercentage": "Double"
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
Content-Length: 254

{
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "id": "65f064cb-64cb-65f0-cb64-f065cb64f065",
  "appDisplayName": "App Display Name value",
  "successfulSignInCount": 5,
  "failedSignInCount": 1,
  "successPercentage": "Double"
}
```

