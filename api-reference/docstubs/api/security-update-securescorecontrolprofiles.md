---
title: "Update secureScoreControlProfiles"
description: "Update the properties of a secureScoreControlProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update secureScoreControlProfiles

Namespace: microsoft.graph

Update the properties of a secureScoreControlProfiles object.

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
PATCH /Security/secureScoreControlProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.

The following table shows the properties that are required when you create the [secureScoreControlProfile](../resources/securescorecontrolprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|actionType|String|**TODO: Add Description**|
|actionUrl|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|complianceInformation|[complianceInformation](../resources/complianceinformation.md) collection|**TODO: Add Description**|
|controlCategory|String|**TODO: Add Description**|
|controlStateUpdates|[secureScoreControlStateUpdate](../resources/securescorecontrolstateupdate.md) collection|**TODO: Add Description**|
|deprecated|Boolean|**TODO: Add Description**|
|implementationCost|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|maxScore|Double|**TODO: Add Description**|
|rank|Int32|**TODO: Add Description**|
|remediation|String|**TODO: Add Description**|
|remediationImpact|String|**TODO: Add Description**|
|service|String|**TODO: Add Description**|
|threats|String collection|**TODO: Add Description**|
|tier|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|userImpact|String|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_securescorecontrolprofiles"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/secureScoreControlProfiles
Content-Type: application/json
Content-length: 1565

{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
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
```

