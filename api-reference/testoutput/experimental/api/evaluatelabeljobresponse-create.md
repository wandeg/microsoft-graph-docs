---
title: "Create evaluateLabelJobResponse"
description: "Create a new evaluateLabelJobResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create evaluateLabelJobResponse

Namespace: microsoft.graph

Create a new [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.

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
POST ** Collection URI for microsoft.graph.evaluateLabelJobResponse not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.

The following table shows the properties that are required when you create the [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|status|String| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|tenantId|String| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|startDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|error|[classificationError](../resources/classificationerror.md)| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|result|[evaluateLabelJobResultGroup](../resources/evaluatelabeljobresultgroup.md)||



## Response
If successful, this method returns a `201 Created` response code and a [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_evaluatelabeljobresponse_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.evaluateLabelJobResponse not found
Content-type: application/json
Content-length: 2325

{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResponse",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2374

{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResponse",
  "id": "283c938f-938f-283c-8f93-3c288f933c28",
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
  }
}
```

