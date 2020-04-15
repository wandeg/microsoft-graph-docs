---
title: "Get provisioningObjectSummary"
description: "Read properties and relationships of the provisioningObjectSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get provisioningObjectSummary

Namespace: Microsoft.AAD.Reporting

Read properties and relationships of the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.

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
GET /auditLogs/provisioning/{provisioningObjectSummaryId}
GET /auditLogs/directoryProvisioning/{provisioningObjectSummaryId}
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
If successful, this method returns a `200 OK` response code and [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_provisioningobjectsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/provisioning/{provisioningObjectSummaryId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.provisioningObjectSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1708

{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
    "id": "848fa6c0-a6c0-848f-c0a6-8f84c0a68f84",
    "activityDateTime": "2016-12-31T23:56:54.8488209+00:00",
    "tenantId": "Tenant Id value",
    "jobId": "Job Id value",
    "cycleId": "Cycle Id value",
    "changeId": "Change Id value",
    "action": "Action value",
    "durationInMilliseconds": 6,
    "initiatedBy": {
      "@odata.type": "Microsoft.AAD.Reporting.initiator",
      "id": "Id value",
      "displayName": "Display Name value",
      "initiatorType": "String"
    },
    "sourceSystem": {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails",
      "details": {
        "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
      }
    },
    "targetSystem": {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
    },
    "sourceIdentity": {
      "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity",
      "identityType": "Identity Type value"
    },
    "targetIdentity": {
      "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
    },
    "statusInfo": {
      "@odata.type": "Microsoft.AAD.Reporting.statusBase",
      "status": "String"
    },
    "provisioningSteps": [
      {
        "@odata.type": "Microsoft.AAD.Reporting.provisioningStep",
        "name": "Name value",
        "description": "Description value",
        "provisioningStepType": "String"
      }
    ],
    "modifiedProperties": [
      {
        "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty",
        "oldValue": "Old Value value",
        "newValue": "New Value value"
      }
    ]
  }
}
```

