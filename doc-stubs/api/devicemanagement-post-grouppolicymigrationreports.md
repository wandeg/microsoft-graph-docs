---
title: "Create groupPolicyMigrationReports"
description: "Create a new groupPolicyMigrationReports object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create groupPolicyMigrationReports

Namespace: microsoft.graph

Create a new groupPolicyMigrationReports object.

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
POST /deviceManagement/groupPolicyMigrationReports
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.

The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|groupPolicyObjectId|Guid|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|ouDistinguishedName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|groupPolicyCreatedDateTime|DateTimeOffset|**TODO: Add Description**|
|groupPolicyLastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|migrationReadiness|groupPolicyMigrationReadiness|**TODO: Add Description**. Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Boolean|**TODO: Add Description**|
|totalSettingsCount|Int32|**TODO: Add Description**|
|supportedSettingsCount|Int32|**TODO: Add Description**|
|supportedSettingsPercent|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicymigrationreport_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
Content-Type: application/json
Content-length: 477

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "Guid",
  "displayName": "String",
  "ouDistinguishedName": "String",
  "groupPolicyCreatedDateTime": "String (timestamp)",
  "groupPolicyLastModifiedDateTime": "String (timestamp)",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": "Boolean",
  "totalSettingsCount": "Integer",
  "supportedSettingsCount": "Integer",
  "supportedSettingsPercent": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicymigrationreport"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "57687ae0-7ae0-5768-e07a-6857e07a6857",
  "groupPolicyObjectId": "Guid",
  "displayName": "String",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "groupPolicyCreatedDateTime": "String (timestamp)",
  "groupPolicyLastModifiedDateTime": "String (timestamp)",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": "Boolean",
  "totalSettingsCount": "Integer",
  "supportedSettingsCount": "Integer",
  "supportedSettingsPercent": "Integer"
}
```

