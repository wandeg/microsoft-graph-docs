---
title: "Add groupPolicyMigrationReports"
description: "Add groupPolicyMigrationReports by posting to the groupPolicyMigrationReports collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add groupPolicyMigrationReports

Namespace: microsoft.graph

Add groupPolicyMigrationReports by posting to the groupPolicyMigrationReports collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.

The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|groupPolicyObjectId|Guid||
|displayName|String||
|ouDistinguishedName|String||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|groupPolicyCreatedDateTime|DateTimeOffset||
|groupPolicyLastModifiedDateTime|DateTimeOffset||
|migrationReadiness|Enumeration| Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Boolean||
|totalSettingsCount|Int32||
|supportedSettingsCount|Int32||
|supportedSettingsPercent|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicymigrationreport_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "b57e6a2e-6a2e-b57e-2e6a-7eb52e6a7eb5",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:51.2750211+03:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:01.4824193+03:00",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicymigrationreport"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 715

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "56ad48fc-48fc-56ad-fc48-ad56fc48ad56",
  "groupPolicyObjectId": "b57e6a2e-6a2e-b57e-2e6a-7eb52e6a7eb5",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:51.2750211+03:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:01.4824193+03:00",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

