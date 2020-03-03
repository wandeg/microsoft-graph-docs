---
title: "Get azureADFeatureUsage"
description: "Read properties and relationships of the azureADFeatureUsage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get azureADFeatureUsage

Namespace: microsoft.graph

Read properties and relationships of the [azureADFeatureUsage](../resources/azureadfeatureusage.md) object.

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
GET ** Entity URI for microsoft.graph.azureADFeatureUsage not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [azureADFeatureUsage](../resources/azureadfeatureusage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_azureadfeatureusage"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.azureADFeatureUsage not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.azureADFeatureUsage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": {
    "@odata.type": "#microsoft.graph.azureADFeatureUsage",
    "id": "dae653c6-53c6-dae6-c653-e6dac653e6da",
    "snapshotDateTime": "2016-12-31T23:56:35.704242+03:00",
    "featureName": "Feature Name value",
    "usage": 5
  }
}
```

