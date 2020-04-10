---
title: "dataClassificationService: classifyExactMatches"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# classifyExactMatches

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
POST /dataClassification/classifyExactMatches
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
|text|String||
|timeoutInMs|String||
|sensitiveTypeIds|String collection||
|contentClassifications|[contentClassification](../resources/contentclassification.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [exactMatchClassificationResult](../resources/exactmatchclassificationresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "dataclassificationservice_classifyexactmatches"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/classifyExactMatches

Content-type: application/json
Content-length: 408

{
  "text": "Text value",
  "timeoutInMs": "Timeout In Ms value",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ],
  "contentClassifications": [
    {
      "@odata.type": "microsoft.graph.contentClassification",
      "sensitiveTypeId": "Sensitive Type Id value",
      "matches": [
        {
          "@odata.type": "microsoft.graph.matchLocation"
        }
      ]
    }
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactmatchclassificationresult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 92

{
  "value": {
    "@odata.type": "microsoft.graph.exactMatchClassificationResult"
  }
}
```

