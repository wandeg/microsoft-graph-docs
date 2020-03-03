---
title: "Create applicationSignInSummary"
description: "Create a new applicationSignInSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create applicationSignInSummary

Namespace: microsoft.graph

Create a new [applicationSignInSummary](../resources/applicationsigninsummary.md) object.

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
POST ** Collection URI for microsoft.graph.applicationSignInSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [applicationSignInSummary](../resources/applicationsigninsummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInSummary](../resources/applicationsigninsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appDisplayName|String||
|successfulSignInCount|Int64||
|failedSignInCount|Int64||
|successPercentage|Double||



## Response
If successful, this method returns a `201 Created` response code and a [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_applicationsigninsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.applicationSignInSummary not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationsigninsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 254

{
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "id": "6d0bb32e-b32e-6d0b-2eb3-0b6d2eb30b6d",
  "appDisplayName": "App Display Name value",
  "successfulSignInCount": 5,
  "failedSignInCount": 1,
  "successPercentage": "Double"
}
```

