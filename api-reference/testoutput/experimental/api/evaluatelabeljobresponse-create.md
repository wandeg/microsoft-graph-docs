---
title: "Create evaluateLabelJobResponse"
description: "Create a new evaluateLabelJobResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create evaluateLabelJobResponse

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
In the request body, supply a JSON representation for the evaluateLabelJobResponse object.

The following table shows the properties that are required when you create the evaluateLabelJobResponse.

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
|result|[evaluateLabelJobResultGroup](../resources/evaluateLabelJobResultGroup.md)||



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
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.evaluateLabelJobResponse not found
Content-type: application/json
Content-length: 2324

{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResponse",
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
Content-Length: 2373

{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResponse",
  "id": "810fe8b8-e8b8-810f-b8e8-0f81b8e80f81",
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

