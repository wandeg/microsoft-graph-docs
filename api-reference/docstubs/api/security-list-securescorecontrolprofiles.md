---
title: "List secureScoreControlProfiles"
description: "Get the secureScoreControlProfiles from the secureScoreControlProfiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List secureScoreControlProfiles

Namespace: microsoft.graph

Get the secureScoreControlProfiles from the secureScoreControlProfiles navigation property.

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
GET /Security/secureScoreControlProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [secureScoreControlProfile](../resources/securescorecontrolprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/secureScoreControlProfiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securescorecontrolprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.secureScoreControlProfile",
      "id": "6303dce7-dce7-6303-e7dc-0363e7dc0363",
      "actionType": "Action Type value",
      "actionUrl": "https://example.com/actionUrl/",
      "azureTenantId": "Azure Tenant Id value",
      "complianceInformation": [
        {
          "@odata.type": "microsoft.graph.complianceInformation",
          "certificationControls": [
            {
              "@odata.type": "microsoft.graph.certificationControl",
              "name": "Name value",
              "url": "Url value"
            }
          ],
          "certificationName": "Certification Name value"
        }
      ],
      "controlCategory": "Control Category value",
      "controlStateUpdates": [
        {
          "@odata.type": "microsoft.graph.secureScoreControlStateUpdate",
          "assignedTo": "Assigned To value",
          "comment": "Comment value",
          "state": "State value",
          "updatedBy": "Updated By value",
          "updatedDateTime": "2017-01-01T00:01:25.2678805+03:00"
        }
      ],
      "deprecated": true,
      "implementationCost": "Implementation Cost value",
      "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
      "maxScore": "Double",
      "rank": 4,
      "remediation": "Remediation value",
      "remediationImpact": "Remediation Impact value",
      "service": "Service value",
      "threats": [
        "Threats value"
      ],
      "tier": "Tier value",
      "title": "Title value",
      "userImpact": "User Impact value",
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation",
        "provider": "Provider value",
        "providerVersion": "Provider Version value",
        "subProvider": "Sub Provider value",
        "vendor": "Vendor value"
      }
    }
  ]
}
```

