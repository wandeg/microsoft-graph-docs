---
title: "Create directoryProvisioning"
description: "Create a new directoryProvisioning object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create directoryProvisioning

Namespace: Microsoft.AAD.Reporting

Create a new directoryProvisioning object.

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
POST /auditLogs/directoryProvisioning
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.

The following table shows the properties that are required when you create the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|jobId|String|**TODO: Add Description**|
|cycleId|String|**TODO: Add Description**|
|changeId|String|**TODO: Add Description**|
|action|String|**TODO: Add Description**|
|durationInMilliseconds|Int32|**TODO: Add Description**|
|servicePrincipal|[provisioningServicePrincipal](../resources/microsoft.aad.reporting-provisioningserviceprincipal.md)|**TODO: Add Description**|
|initiatedBy|[initiator](../resources/microsoft.aad.reporting-initiator.md)|**TODO: Add Description**|
|sourceSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)|**TODO: Add Description**|
|targetSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)|**TODO: Add Description**|
|sourceIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)|**TODO: Add Description**|
|targetIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)|**TODO: Add Description**|
|statusInfo|[statusBase](../resources/microsoft.aad.reporting-statusbase.md)|**TODO: Add Description**|
|provisioningSteps|[provisioningStep](../resources/microsoft.aad.reporting-provisioningstep.md) collection|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_provisioningobjectsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
Content-Type: application/json
Content-length: 1646

{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "activityDateTime": "2017-01-01T00:03:11.0875532+00:00",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.aad.reporting.provisioningobjectsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "id": "1af8a3ef-a3ef-1af8-efa3-f81aefa3f81a",
  "activityDateTime": "2017-01-01T00:03:11.0875532+00:00",
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
```

