---
title: "Create complianceManagementPartners"
description: "Create a new complianceManagementPartners object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create complianceManagementPartners

Namespace: microsoft.graph

Create a new complianceManagementPartners object.

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
POST /deviceManagement/complianceManagementPartners
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.

The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/compliancemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset|**TODO: Add Description**|
|partnerState|deviceManagementPartnerTenantState|**TODO: Add Description**. Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|displayName|String|**TODO: Add Description**|
|macOsOnboarded|Boolean|**TODO: Add Description**|
|windowsOnboarded|Boolean|**TODO: Add Description**|
|androidOnboarded|Boolean|**TODO: Add Description**|
|iosOnboarded|Boolean|**TODO: Add Description**|
|macOsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|**TODO: Add Description**|
|windowsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|**TODO: Add Description**|
|androidEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|**TODO: Add Description**|
|iosEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/compliancemanagementpartner.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_compliancemanagementpartner_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
Content-Type: application/json
Content-length: 840

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "displayName": "String",
  "macOsOnboarded": "Boolean",
  "windowsOnboarded": "Boolean",
  "androidOnboarded": "Boolean",
  "iosOnboarded": "Boolean",
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.compliancemanagementpartner"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "a68cb08c-b08c-a68c-8cb0-8ca68cb08ca6",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "displayName": "String",
  "macOsOnboarded": "Boolean",
  "windowsOnboarded": "Boolean",
  "androidOnboarded": "Boolean",
  "iosOnboarded": "Boolean",
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ]
}
```

