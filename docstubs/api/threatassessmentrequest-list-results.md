---
title: "List results"
description: "Get the threatAssessmentResults from the results navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List results

Namespace: microsoft.graph

Get the threatAssessmentResults from the results navigation property.

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
GET /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentResult](../resources/threatassessmentresult.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.threatassessmentresult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 283

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.threatAssessmentResult",
      "id": "0082208f-208f-0082-8f20-82008f208200",
      "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
      "resultType": "String",
      "message": "Message value"
    }
  ]
}
```

