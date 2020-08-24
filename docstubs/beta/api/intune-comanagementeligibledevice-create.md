---
title: "Create comanagementEligibleDevice"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create comanagementEligibleDevice

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new comanagementEligibleDevice object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the comanagementEligibleDevice object.

The following table shows the properties that are required when you create the comanagementEligibleDevice object.

| Property                 | Type                           | Description                           |
| :----------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name)  | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |
| clientRegistrationStatus | String                         | ClientRegistrationStatus              |
| deviceName               | String                         | DeviceName                            |
| deviceType               | String                         | DeviceType                            |
| entitySource             | Int32                          | EntitySource                          |
| id                       | String                         | Unique Id for the device Read-only.   |
| managementAgents         | String                         | ManagementAgents                      |
| managementState          | String                         | ManagementState                       |
| manufacturer             | String                         | Manufacturer                          |
| mdmStatus                | String                         | MDMStatus                             |
| model                    | String                         | Model                                 |
| osDescription            | String                         | OSDescription                         |
| osVersion                | String                         | OSVersion                             |
| ownerType                | String                         | OwnerType                             |
| referenceId              | String                         | ReferenceId                           |
| serialNumber             | String                         | SerialNumber                          |
| status                   | String                         | ComanagementEligibleStatus            |
| upn                      | String                         | UPN                                   |
| userEmail                | String                         | UserEmail                             |
| userId                   | String                         | UserId                                |
| userName                 | String                         | UserName                              |

Do not supply a request body for this method.

## Response

If successful, this method returns a `201 Created` response code and a [comanagementEligibleDevice](../resources/comanagementEligibleDevice.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_comanagementeligibledevice"
}
-->

```http
POST https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 589

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "clientRegistrationStatus": "String",
  "deviceName": "String",
  "deviceType": "String",
  "entitySource": "Int32",
  "managementAgents": "String",
  "managementState": "String",
  "manufacturer": "String",
  "mdmStatus": "String",
  "model": "String",
  "osDescription": "String",
  "osVersion": "String",
  "ownerType": "String",
  "referenceId": "String",
  "serialNumber": "String",
  "status": "String",
  "upn": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.comanagementEligibleDevice"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "clientRegistrationStatus": "String",
  "deviceName": "String",
  "deviceType": "String",
  "entitySource": "Int32",
  "id": "String(identifier)",
  "managementAgents": "String",
  "managementState": "String",
  "manufacturer": "String",
  "mdmStatus": "String",
  "model": "String",
  "osDescription": "String",
  "osVersion": "String",
  "ownerType": "String",
  "referenceId": "String",
  "serialNumber": "String",
  "status": "String",
  "upn": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String"
}
}

```