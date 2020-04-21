---
title: "Update domain"
description: "Update the properties of a domain object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update domain

Namespace: microsoft.graph

Update the properties of a [domain](../resources/domain.md) object.

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
PATCH /domains/{domainsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [domain](../resources/domain.md) object.

The following table shows the properties that are required when you create the [domain](../resources/domain.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|authenticationType|String|**TODO: Add Description**|
|availabilityStatus|String|**TODO: Add Description**|
|isAdminManaged|Boolean|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|isInitial|Boolean|**TODO: Add Description**|
|isRoot|Boolean|**TODO: Add Description**|
|isVerified|Boolean|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|passwordNotificationWindowInDays|Int32|**TODO: Add Description**|
|passwordValidityPeriodInDays|Int32|**TODO: Add Description**|
|supportedServices|String collection|**TODO: Add Description**|
|state|[domainState](../resources/domainstate.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [domain](../resources/domain.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_domain"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/domains/{domainsId}
Content-Type: application/json
Content-length: 683

{
  "@odata.type": "#microsoft.graph.domain",
  "authenticationType": "Authentication Type value",
  "availabilityStatus": "Availability Status value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "passwordNotificationWindowInDays": 0,
  "passwordValidityPeriodInDays": 12,
  "supportedServices": [
    "Supported Services value"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "Status value",
    "operation": "Operation value",
    "lastActionDateTime": "2017-01-01T00:00:26.005933+00:00"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.domain",
  "id": "56655a11-5a11-5665-115a-6556115a6556",
  "authenticationType": "Authentication Type value",
  "availabilityStatus": "Availability Status value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "passwordNotificationWindowInDays": 0,
  "passwordValidityPeriodInDays": 12,
  "supportedServices": [
    "Supported Services value"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "Status value",
    "operation": "Operation value",
    "lastActionDateTime": "2017-01-01T00:00:26.005933+00:00"
  }
}
```

