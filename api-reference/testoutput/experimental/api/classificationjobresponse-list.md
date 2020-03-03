---
title: "List classificationJobResponses"
description: "List properties and relationships of the classificationJobResponse objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List classificationJobResponses

List properties and relationships of the [classificationJobResponse](../resources/classificationjobresponse.md) objects.

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
GET ** Collection URI for microsoft.graph.classificationJobResponse not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [classificationJobResponse](../resources/classificationjobresponse.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_classificationjobresponse"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.classificationJobResponse not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.classificationjobresponse)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1965

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.classificationJobResponse",
      "id": "135d6e53-6e53-135d-536e-5d13536e5d13",
      "type": "Type value",
      "status": "Status value",
      "tenantId": "Tenant Id value",
      "creationDateTime": "2017-01-01T00:00:59.0982804+03:00",
      "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
      "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
      "error": {
        "@odata.type": "microsoft.graph.classificationError",
        "code": "Code value",
        "message": "Message value",
        "target": "Target value",
        "innerError": {
          "@odata.type": "microsoft.graph.classificationInnerError",
          "errorDateTime": "2017-01-01T00:03:21.298689+03:00",
          "clientRequestId": "Client Request Id value",
          "activityId": "Activity Id value"
        },
        "details": [
          {
            "@odata.type": "microsoft.graph.classifcationErrorBase"
          }
        ]
      },
      "result": {
        "@odata.type": "microsoft.graph.detectedSensitiveContentWrapper",
        "classification": [
          {
            "@odata.type": "microsoft.graph.detectedSensitiveContent",
            "id": "7fa8665d-665d-7fa8-5d66-a87f5d66a87f",
            "displayName": "Display Name value",
            "uniqueCount": 11,
            "confidence": 10,
            "recommendedConfidence": 5,
            "matches": [
              {
                "@odata.type": "microsoft.graph.sensitiveContentLocation",
                "idMatch": "Id Match value",
                "offset": 6,
                "length": 6,
                "evidences": [
                  {
                    "@odata.type": "microsoft.graph.sensitiveContentEvidence",
                    "match": "Match value"
                  }
                ]
              }
            ]
          }
        ]
      }
    }
  ]
}
```

