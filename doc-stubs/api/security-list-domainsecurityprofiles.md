---
title: "List domainSecurityProfiles"
description: "Get the domainSecurityProfiles from the domainSecurityProfiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List domainSecurityProfiles

Namespace: microsoft.graph

Get the domainSecurityProfiles from the domainSecurityProfiles navigation property.

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
GET /Security/domainSecurityProfiles
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

If successful, this method returns a `200 OK` response code and a collection of [domainSecurityProfile](../resources/domainsecurityprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domainsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/domainSecurityProfiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domainsecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domainSecurityProfile",
      "id": "cb4fac94-ac94-cb4f-94ac-4fcb94ac4fcb",
      "activityGroupNames": [
        "String"
      ],
      "azureSubscriptionId": "String",
      "azureTenantId": "String",
      "countHits": "Integer",
      "countInOrg": "Integer",
      "domainCategories": [
        {
          "@odata.type": "microsoft.graph.reputationCategory"
        }
      ],
      "domainRegisteredDateTime": "String (timestamp)",
      "firstSeenDateTime": "String (timestamp)",
      "lastSeenDateTime": "String (timestamp)",
      "name": "String",
      "registrant": {
        "@odata.type": "microsoft.graph.domainRegistrant"
      },
      "riskScore": "String",
      "tags": [
        "String"
      ],
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation"
      }
    }
  ]
}
```

