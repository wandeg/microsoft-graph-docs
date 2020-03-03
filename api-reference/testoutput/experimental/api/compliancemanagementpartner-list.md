---
title: "List complianceManagementPartners"
description: "List properties and relationships of the complianceManagementPartner objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List complianceManagementPartners

Namespace: microsoft.graph

List properties and relationships of the [complianceManagementPartner](../resources/compliancemanagementpartner.md) objects.

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
GET /deviceManagement/complianceManagementPartners
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/compliancemanagementpartner.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_compliancemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/complianceManagementPartners
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
      "id": "5c7bae0f-ae0f-5c7b-0fae-7b5c0fae7b5c",
      "lastHeartbeatDateTime": "2016-12-31T23:57:32.1210231+03:00",
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

