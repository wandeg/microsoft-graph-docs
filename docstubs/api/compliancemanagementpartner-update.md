---
title: "Update complianceManagementPartner"
description: "Update the properties of a complianceManagementPartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update complianceManagementPartner

Namespace: microsoft.graph

Update the properties of a [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.

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
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.

The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/compliancemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset||
|partnerState|Enumeration| Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|displayName|String||
|macOsOnboarded|Boolean||
|windowsOnboarded|Boolean||
|androidOnboarded|Boolean||
|iosOnboarded|Boolean||
|macOsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection||
|windowsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection||
|androidEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection||
|iosEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/compliancemanagementpartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_compliancemanagementpartner"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 951

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2017-01-01T00:00:12.4442527+03:00",
  "partnerState": "String",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      }
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "8ad1eb04-eb04-8ad1-04eb-d18a04ebd18a",
  "lastHeartbeatDateTime": "2017-01-01T00:00:12.4442527+03:00",
  "partnerState": "String",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      }
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

