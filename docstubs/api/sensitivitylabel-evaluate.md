---
title: "evaluate"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# evaluate

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
POST /dataClassification/sensitivityLabels/evaluate
POST /informationProtection/sensitivityLabels/evaluate
POST /dataClassification/sensitivityLabels/{sensitivityLabelId}/sublabels/evaluate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|discoveredSensitiveTypes|[discoveredSensitiveType](../resources/discoveredsensitivetype.md) collection||
|currentLabel|[currentLabel](../resources/currentlabel.md)||



## Response
If successful, this action returns a `200 OK` response code and a [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "sensitivitylabel_evaluate"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/sensitivityLabels/evaluate

Content-type: application/json
Content-length: 295

{
  "discoveredSensitiveTypes": [
    {
      "@odata.type": "microsoft.graph.discoveredSensitiveType",
      "id": "929cad84-ad84-929c-84ad-9c9284ad9c92",
      "count": 5,
      "confidence": 10
    }
  ],
  "currentLabel": {
    "@odata.type": "microsoft.graph.currentLabel"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.evaluatelabeljobresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 587

{
  "value": {
    "@odata.type": "#microsoft.graph.evaluateLabelJobResponse",
    "id": "9c1b19af-19af-9c1b-af19-1b9caf191b9c",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2017-01-01T00:01:50.3140554+03:00",
    "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
    "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.evaluateLabelJobResultGroup"
    }
  }
}
```

