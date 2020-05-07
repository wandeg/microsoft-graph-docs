---
title: "Create deviceConfigurationConflictSummary"
description: "Create a new deviceConfigurationConflictSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceConfigurationConflictSummary

Namespace: microsoft.graph

Create a new deviceConfigurationConflictSummary object.

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
POST /deviceManagement/deviceConfigurationConflictSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|conflictingDeviceConfigurations|[settingSource](../resources/settingsource.md) collection|**TODO: Add Description**|
|contributingSettings|String collection|**TODO: Add Description**|
|deviceCheckinsImpacted|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deviceconfigurationconflictsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-Type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource"
    }
  ],
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceconfigurationconflictsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "id": "232ef2ca-f2ca-232e-caf2-2e23caf22e23",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource"
    }
  ],
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": "Integer"
}
```

