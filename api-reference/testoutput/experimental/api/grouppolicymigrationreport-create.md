---
title: "Create groupPolicyMigrationReport"
description: "Create a new groupPolicyMigrationReport object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create groupPolicyMigrationReport

Namespace: microsoft.graph

Create a new [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.

The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|groupPolicyObjectId|Guid|The Group Policy Object GUID from GPO Xml content|
|displayName|String|The name of Group Policy Object from the GPO Xml Content|
|ouDistinguishedName|String|The distinguished name of the OU.|
|createdDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was created.|
|lastModifiedDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was last modified.|
|groupPolicyCreatedDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was created.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was last modified.|
|migrationReadiness|Enumeration|The Intune coverage for the associated Group Policy Object file. Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Boolean|The Targeted in AD property from GPO Xml Content|
|totalSettingsCount|Int32|The total number of Group Policy Settings from GPO file.|
|supportedSettingsCount|Int32|The number of Group Policy Settings supported by Intune.|
|supportedSettingsPercent|Int32|The Percentage of Group Policy Settings supported by Intune.|



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicymigrationreport_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/groupPolicyMigrationReports
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "1713d55d-d55d-1713-5dd5-13175dd51317",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2017-01-01T00:01:08.1552648+03:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:03:02.9368554+03:00",
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
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "f08ed319-d319-f08e-19d3-8ef019d38ef0",
  "groupPolicyObjectId": "1713d55d-d55d-1713-5dd5-13175dd51317",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "groupPolicyCreatedDateTime": "2017-01-01T00:01:08.1552648+03:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:03:02.9368554+03:00",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

