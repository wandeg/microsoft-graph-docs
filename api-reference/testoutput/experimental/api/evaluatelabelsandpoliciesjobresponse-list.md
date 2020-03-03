---
title: "List evaluateLabelsAndPoliciesJobResponses"
description: "List properties and relationships of the evaluateLabelsAndPoliciesJobResponse objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List evaluateLabelsAndPoliciesJobResponses

Namespace: microsoft.graph

List properties and relationships of the [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) objects.

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
GET ** Collection URI for microsoft.graph.evaluateLabelsAndPoliciesJobResponse not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_evaluatelabelsandpoliciesjobresponse"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.evaluateLabelsAndPoliciesJobResponse not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.evaluatelabelsandpoliciesjobresponse)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4544

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesJobResponse",
      "id": "b61f2273-2273-b61f-7322-1fb673221fb6",
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
        "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult",
        "sensitivityLabelsResult": {
          "@odata.type": "microsoft.graph.evaluateLabelJobResultGroup",
          "automatic": {
            "@odata.type": "microsoft.graph.evaluateLabelJobResult",
            "sensitivityLabel": {
              "@odata.type": "microsoft.graph.matchingLabel",
              "id": "Id value",
              "name": "Name value",
              "displayName": "Display Name value",
              "description": "Description value",
              "toolTip": "Tool Tip value",
              "policyTip": "Policy Tip value",
              "isEndpointProtectionEnabled": true,
              "applicationMode": "String",
              "labelActions": [
                {
                  "@odata.type": "microsoft.graph.encryptWithUserDefinedRights",
                  "encryptWith": "String",
                  "decryptionRightsManagementTemplateId": "Decryption Rights Management Template Id value",
                  "allowMailForwarding": true,
                  "allowAdHocPermissions": true
                }
              ],
              "priority": 8
            },
            "responsibleSensitiveTypes": [
              {
                "@odata.type": "microsoft.graph.responsibleSensitiveType",
                "rulePackageId": "Rule Package Id value",
                "rulePackageType": "Rule Package Type value",
                "publisherName": "Publisher Name value"
              }
            ],
            "responsiblePolicy": {
              "@odata.type": "microsoft.graph.responsiblePolicy"
            }
          },
          "recommended": {
            "@odata.type": "microsoft.graph.evaluateLabelJobResult"
          }
        },
        "dataLossPreventionPoliciesResult": {
          "@odata.type": "microsoft.graph.dlpPoliciesJobResult",
          "matchingRules": [
            {
              "@odata.type": "microsoft.graph.matchingDlpRule",
              "ruleId": "Rule Id value",
              "ruleName": "Rule Name value",
              "policyId": "Policy Id value",
              "policyName": "Policy Name value",
              "isMostRestrictive": true,
              "actions": [
                {
                  "@odata.type": "microsoft.graph.dlpActionInfo",
                  "action": "String"
                }
              ],
              "ruleMode": "String"
            }
          ]
        },
        "classificationResult": {
          "@odata.type": "microsoft.graph.detectedSensitiveContentWrapper",
          "classification": [
            {
              "@odata.type": "microsoft.graph.detectedSensitiveContent",
              "id": "cdc6f9dc-f9dc-cdc6-dcf9-c6cddcf9c6cd",
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
    }
  ]
}
```

