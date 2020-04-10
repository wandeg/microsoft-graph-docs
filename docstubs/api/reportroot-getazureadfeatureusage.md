---
title: "reportRoot: getAzureADFeatureUsage"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getAzureADFeatureUsage

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
GET /reports/getAzureADFeatureUsage
GET /print/reports/{reportRootId}/getAzureADFeatureUsage
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
If successful, this function returns a `200 OK` response code and a [azureADFeatureUsage](../resources/azureadfeatureusage.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getazureadfeatureusage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAzureADFeatureUsage(period='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.azureadfeatureusage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.azureADFeatureUsage",
      "id": "ba2dd66d-d66d-ba2d-6dd6-2dba6dd62dba",
      "snapshotDateTime": "2017-01-01T00:01:40.0897462+00:00",
      "featureName": "Feature Name value",
      "usage": 5
    }
  ]
}
```

