---
title: "Create secureScoreControlProfiles"
description: "Create a new secureScoreControlProfiles object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create secureScoreControlProfiles

Namespace: microsoft.graph

Create a new secureScoreControlProfiles object.

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
POST /Security/secureScoreControlProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.

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
If successful, this method returns a `201 Created` response code and a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_securescorecontrolprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/secureScoreControlProfiles
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
      "updatedDateTime": "2016-12-31T23:58:27.5767592+00:00"
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securescorecontrolprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
  "id": "b7203155-3155-b720-5531-20b7553120b7",
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
      "updatedDateTime": "2016-12-31T23:58:27.5767592+00:00"
    }
  ],
  "deprecated": true,
  "implementationCost": "Implementation Cost value",
  "lastModifiedDateTime": "2017-01-01T00:01:26.0388723+00:00",
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

