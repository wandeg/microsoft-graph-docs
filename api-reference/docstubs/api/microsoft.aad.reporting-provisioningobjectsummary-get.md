---
title: "Get provisioningObjectSummary"
description: "Read properties and relationships of a provisioningObjectSummary object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get provisioningObjectSummary

Namespace: Microsoft.AAD.Reporting

Read properties and relationships of a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object in the response body.

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
{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
    "id": "0b715cef-5cef-0b71-ef5c-710bef5c710b",
    "activityDateTime": "2017-01-01T00:01:43.992962+03:00",
    "tenantId": "Tenant Id value",
    "jobId": "Job Id value",
    "cycleId": "Cycle Id value",
    "changeId": "Change Id value",
    "action": "Action value",
    "durationInMilliseconds": 6,
    "servicePrincipal": {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningServicePrincipal",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "initiatedBy": {
      "@odata.type": "Microsoft.AAD.Reporting.initiator",
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

