---
title: "Update provisioning"
description: "Update the properties of a provisioning object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update provisioning

Namespace: Microsoft.AAD.Reporting

Update the properties of a provisioning object.

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
PATCH /auditLogs/provisioning
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.

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
|initiatedBy|[initiator](../resources/microsoft.aad.reporting-initiator.md)|**TODO: Add Description**|
|sourceSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)|**TODO: Add Description**|
|targetSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)|**TODO: Add Description**|
|sourceIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)|**TODO: Add Description**|
|targetIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)|**TODO: Add Description**|
|statusInfo|[statusBase](../resources/microsoft.aad.reporting-statusbase.md)|**TODO: Add Description**|
|provisioningSteps|[provisioningStep](../resources/microsoft.aad.reporting-provisioningstep.md) collection|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_provisioning"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/provisioning
Content-Type: application/json
Content-length: 1054

{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "activityDateTime": "String (timestamp)",
  "tenantId": "String",
  "jobId": "String",
  "cycleId": "String",
  "changeId": "String",
  "action": "String",
  "durationInMilliseconds": "Integer",
  "initiatedBy": {
    "@odata.type": "Microsoft.AAD.Reporting.initiator"
  },
  "sourceSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "targetSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "targetIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "Microsoft.AAD.Reporting.statusBase"
  },
  "provisioningSteps": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningStep"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "id": "d2bacca6-cca6-d2ba-a6cc-bad2a6ccbad2",
  "activityDateTime": "String (timestamp)",
  "tenantId": "String",
  "jobId": "String",
  "cycleId": "String",
  "changeId": "String",
  "action": "String",
  "durationInMilliseconds": "Integer",
  "initiatedBy": {
    "@odata.type": "Microsoft.AAD.Reporting.initiator"
  },
  "sourceSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "targetSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "targetIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "Microsoft.AAD.Reporting.statusBase"
  },
  "provisioningSteps": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningStep"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty"
    }
  ]
}
```

