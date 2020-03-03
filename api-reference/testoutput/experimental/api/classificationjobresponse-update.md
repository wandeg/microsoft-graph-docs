---
title: "Update classificationJobResponse"
description: "Update the properties of a classificationJobResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update classificationJobResponse

Update the properties of a [classificationJobResponse](../resources/classificationjobresponse.md) object.

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
PATCH ** Entity URI for microsoft.graph.classificationJobResponse not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [classificationJobResponse](../resources/classificationJobResponse.md) object.

The following table shows the properties that are required when you create the [classificationJobResponse](../resources/classificationjobresponse.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|status|String| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|tenantId|String| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|startDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|error|[classificationError](../resources/classificationError.md)| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|result|[detectedSensitiveContentWrapper](../resources/detectedSensitiveContentWrapper.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [classificationJobResponse](../resources/classificationjobresponse.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_classificationjobresponse"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.classificationJobResponse not found
Content-type: application/json
Content-length: 1675

{
  "@odata.type": "#microsoft.graph.classificationJobResponse",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1724

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
```

