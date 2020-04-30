---
title: "Add homeRealmDiscoveryPolicies"
description: "Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Add homeRealmDiscoveryPolicies

Namespace: Microsoft.DirectoryServices

Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.

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
POST /servicePrincipals/{servicePrincipalsId}/homeRealmDiscoveryPolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md) object.

The following table shows the properties that are required when you create the [homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/microsoft.directoryservices-stspolicy.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/microsoft.directoryservices-stspolicy.md)|



## Response
If successful, this method returns a `204 No Content` response code and a [homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/servicePrincipals/{servicePrincipalsId}/homeRealmDiscoveryPolicies/$ref
Content-Type: application/json
Content-length: 240

{
  "@odata.type": "#Microsoft.DirectoryServices.homeRealmDiscoveryPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.homerealmdiscoverypolicy"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.homeRealmDiscoveryPolicy",
  "id": "ce89159c-159c-ce89-9c15-89ce9c1589ce",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

