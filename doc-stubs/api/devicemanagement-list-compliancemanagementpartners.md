---
title: "List complianceManagementPartners"
description: "Get the complianceManagementPartners from the complianceManagementPartners navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List complianceManagementPartners

Namespace: microsoft.graph

Get the complianceManagementPartners from the complianceManagementPartners navigation property.

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
GET /deviceManagement/complianceManagementPartners
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/compliancemanagementpartner.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_compliancemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.compliancemanagementpartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

