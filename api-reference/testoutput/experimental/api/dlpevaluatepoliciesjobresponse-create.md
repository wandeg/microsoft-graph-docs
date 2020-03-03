---
title: "Create dlpEvaluatePoliciesJobResponse"
description: "Create a new dlpEvaluatePoliciesJobResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create dlpEvaluatePoliciesJobResponse

Create a new [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object.

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
POST ** Collection URI for microsoft.graph.dlpEvaluatePoliciesJobResponse not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the dlpEvaluatePoliciesJobResponse object.

The following table shows the properties that are required when you create the dlpEvaluatePoliciesJobResponse.

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
|result|[dlpPoliciesJobResult](../resources/dlpPoliciesJobResult.md)||



## Response
If successful, this method returns a `201 Created` response code and a [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_dlpevaluatepoliciesjobresponse_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.dlpEvaluatePoliciesJobResponse not found
Content-type: application/json
Content-length: 1451

{
  "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
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
    "@odata.type": "microsoft.graph.dlpPoliciesJobResult",
    "matchingRules": [
      {
        "@odata.type": "microsoft.graph.matchingDlpRule",
        "ruleId": "Rule Id value",
        "ruleName": "Rule Name value",
        "policyId": "Policy Id value",
        "policyName": "Policy Name value",
        "isMostRestrictive": true,
        "priority": 8,
        "actions": [
          {
            "@odata.type": "microsoft.graph.dlpActionInfo",
            "action": "String"
          }
        ],
        "ruleMode": "String"
      }
    ]
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dlpevaluatepoliciesjobresponse"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1500

{
  "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
  "id": "6785a295-a295-6785-95a2-856795a28567",
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
    "@odata.type": "microsoft.graph.dlpPoliciesJobResult",
    "matchingRules": [
      {
        "@odata.type": "microsoft.graph.matchingDlpRule",
        "ruleId": "Rule Id value",
        "ruleName": "Rule Name value",
        "policyId": "Policy Id value",
        "policyName": "Policy Name value",
        "isMostRestrictive": true,
        "priority": 8,
        "actions": [
          {
            "@odata.type": "microsoft.graph.dlpActionInfo",
            "action": "String"
          }
        ],
        "ruleMode": "String"
      }
    ]
  }
}
```

