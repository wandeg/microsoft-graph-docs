---
title: "Get threatAssessmentResult"
description: "Read properties and relationships of the threatAssessmentResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get threatAssessmentResult

Namespace: microsoft.graph

Read properties and relationships of the [threatAssessmentResult](../resources/threatassessmentresult.md) object.

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
GET /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/{threatAssessmentResultId}
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
If successful, this method returns a `200 OK` response code and [threatAssessmentResult](../resources/threatassessmentresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/{threatAssessmentResultId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatAssessmentResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": {
    "@odata.type": "#microsoft.graph.threatAssessmentResult",
    "id": "88de20c2-20c2-88de-c220-de88c220de88",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "resultType": "String",
    "message": "Message value"
  }
}
```

