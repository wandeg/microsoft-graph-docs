---
title: "List complianceManagementPartners"
description: "Get the complianceManagementPartners from the complianceManagementPartners navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List complianceManagementPartners

Namespace: microsoft.graph

Get the complianceManagementPartners from the complianceManagementPartners navigation property.

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
GET /deviceManagement/complianceManagementPartners
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
If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/compliancemanagementpartner.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_compliancemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.compliancemanagementpartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1161

{
  "value": [
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
  ]
}
```

