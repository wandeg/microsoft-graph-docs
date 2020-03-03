---
title: "List threatAssessmentResults"
description: "List properties and relationships of the threatAssessmentResult objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List threatAssessmentResults

Namespace: microsoft.graph

List properties and relationships of the [threatAssessmentResult](../resources/threatassessmentresult.md) objects.

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
GET /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentResult](../resources/threatassessmentresult.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentresult"
}
-->
``` http
GET https://graph.microsoft.com/localtest/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
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
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.threatAssessmentResult",
      "id": "547f34d2-34d2-547f-d234-7f54d2347f54",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "resultType": "String",
      "message": "Message value"
    }
  ]
}
```

