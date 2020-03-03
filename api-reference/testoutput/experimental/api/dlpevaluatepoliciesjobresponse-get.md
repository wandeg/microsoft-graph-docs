---
title: "Get dlpEvaluatePoliciesJobResponse"
description: "Read properties and relationships of the dlpEvaluatePoliciesJobResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get dlpEvaluatePoliciesJobResponse

Namespace: microsoft.graph

Read properties and relationships of the [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object.

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
GET ** Entity URI for microsoft.graph.dlpEvaluatePoliciesJobResponse not found
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
If successful, this method returns a `200 OK` response code and [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_dlpevaluatepoliciesjobresponse"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.dlpEvaluatePoliciesJobResponse not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dlpEvaluatePoliciesJobResponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1612

{
  "value": {
    "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
    "id": "59329ea6-9ea6-5932-a69e-3259a69e3259",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
    "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
    "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError",
      "code": "Code value",
      "message": "Message value",
      "target": "Target value",
      "innerError": {
        "@odata.type": "microsoft.graph.classificationInnerError",
        "errorDateTime": "2016-12-31T23:59:22.9712113+03:00",
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
}
```

