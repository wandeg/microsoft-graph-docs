---
title: "Add complianceManagementPartners"
description: "Add complianceManagementPartners by posting to the complianceManagementPartners collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add complianceManagementPartners

Namespace: microsoft.graph

Add complianceManagementPartners by posting to the complianceManagementPartners collection.

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
POST /deviceManagement/complianceManagementPartners/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/compliancemanagementpartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_compliancemanagementpartner_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 951

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:56:56.7799755+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.compliancemanagementpartner"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1000

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "0c65e46a-e46a-0c65-6ae4-650c6ae4650c",
  "lastHeartbeatDateTime": "2016-12-31T23:56:56.7799755+03:00",
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

