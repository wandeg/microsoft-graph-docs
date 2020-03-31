---
title: "getAzureADApplicationSignInSummary"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getAzureADApplicationSignInSummary

Namespace: microsoft.graph



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
GET /reports/getAzureADApplicationSignInSummary
GET /print/reports/{reportRootId}/getAzureADApplicationSignInSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [applicationSignInSummary](../resources/applicationsigninsummary.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getazureadapplicationsigninsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.applicationsigninsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applicationSignInSummary",
      "id": "504740c1-40c1-5047-c140-4750c1404750",
      "appDisplayName": "App Display Name value",
      "successfulSignInCount": 5,
      "failedSignInCount": 1,
      "successPercentage": "Double"
    }
  ]
}
```

