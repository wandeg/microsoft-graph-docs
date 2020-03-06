---
title: "security resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# security resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get security](../api/security-get.md)|[security](../resources/security.md)|Read properties and relationships of the [security](../resources/security.md) object.|
|[Update security](../api/security-update.md)|[security](../resources/security.md)|Update the properties of a [security](../resources/security.md) object.|
|[List alerts](../api/security-list-alerts.md)|[alert](../resources/alert.md) collection|Get the alerts from the alerts navigation property.|
|[Add alerts](../api/security-post-alerts.md)|[alert](../resources/alert.md)|Add alerts by posting to the alerts collection.|
|[List cloudAppSecurityProfiles](../api/security-list-cloudappsecurityprofiles.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) collection|Get the cloudAppSecurityProfiles from the cloudAppSecurityProfiles navigation property.|
|[Add cloudAppSecurityProfiles](../api/security-post-cloudappsecurityprofiles.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Add cloudAppSecurityProfiles by posting to the cloudAppSecurityProfiles collection.|
|[List domainSecurityProfiles](../api/security-list-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md) collection|Get the domainSecurityProfiles from the domainSecurityProfiles navigation property.|
|[Add domainSecurityProfiles](../api/security-post-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Add domainSecurityProfiles by posting to the domainSecurityProfiles collection.|
|[List fileSecurityProfiles](../api/security-list-filesecurityprofiles.md)|[fileSecurityProfile](../resources/filesecurityprofile.md) collection|Get the fileSecurityProfiles from the fileSecurityProfiles navigation property.|
|[Add fileSecurityProfiles](../api/security-post-filesecurityprofiles.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Add fileSecurityProfiles by posting to the fileSecurityProfiles collection.|
|[List hostSecurityProfiles](../api/security-list-hostsecurityprofiles.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md) collection|Get the hostSecurityProfiles from the hostSecurityProfiles navigation property.|
|[Add hostSecurityProfiles](../api/security-post-hostsecurityprofiles.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Add hostSecurityProfiles by posting to the hostSecurityProfiles collection.|
|[List ipSecurityProfiles](../api/security-list-ipsecurityprofiles.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md) collection|Get the ipSecurityProfiles from the ipSecurityProfiles navigation property.|
|[Add ipSecurityProfiles](../api/security-post-ipsecurityprofiles.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md)|Add ipSecurityProfiles by posting to the ipSecurityProfiles collection.|
|[List providerTenantSettings](../api/security-list-providertenantsettings.md)|[providerTenantSetting](../resources/providertenantsetting.md) collection|Get the providerTenantSettings from the providerTenantSettings navigation property.|
|[Add providerTenantSettings](../api/security-post-providertenantsettings.md)|[providerTenantSetting](../resources/providertenantsetting.md)|Add providerTenantSettings by posting to the providerTenantSettings collection.|
|[List secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|Get the secureScoreControlProfiles from the secureScoreControlProfiles navigation property.|
|[Add secureScoreControlProfiles](../api/security-post-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Add secureScoreControlProfiles by posting to the secureScoreControlProfiles collection.|
|[List secureScores](../api/security-list-securescores.md)|[secureScore](../resources/securescore.md) collection|Get the secureScores from the secureScores navigation property.|
|[Add secureScores](../api/security-post-securescores.md)|[secureScore](../resources/securescore.md)|Add secureScores by posting to the secureScores collection.|
|[List tiIndicators](../api/security-list-tiindicators.md)|[tiIndicator](../resources/tiindicator.md) collection|Get the tiIndicators from the tiIndicators navigation property.|
|[Add tiIndicators](../api/security-post-tiindicators.md)|[tiIndicator](../resources/tiindicator.md)|Add tiIndicators by posting to the tiIndicators collection.|
|[List userSecurityProfiles](../api/security-list-usersecurityprofiles.md)|[userSecurityProfile](../resources/usersecurityprofile.md) collection|Get the userSecurityProfiles from the userSecurityProfiles navigation property.|
|[Add userSecurityProfiles](../api/security-post-usersecurityprofiles.md)|[userSecurityProfile](../resources/usersecurityprofile.md)|Add userSecurityProfiles by posting to the userSecurityProfiles collection.|
|[List securityActions](../api/security-list-securityactions.md)|[securityAction](../resources/securityaction.md) collection|Get the securityActions from the securityActions navigation property.|
|[Add securityActions](../api/security-post-securityactions.md)|[securityAction](../resources/securityaction.md)|Add securityActions by posting to the securityActions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|providerStatus|[securityProviderStatus](../resources/securityproviderstatus.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|alerts|[alert](../resources/alert.md) collection||
|cloudAppSecurityProfiles|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) collection||
|domainSecurityProfiles|[domainSecurityProfile](../resources/domainsecurityprofile.md) collection||
|fileSecurityProfiles|[fileSecurityProfile](../resources/filesecurityprofile.md) collection||
|hostSecurityProfiles|[hostSecurityProfile](../resources/hostsecurityprofile.md) collection||
|ipSecurityProfiles|[ipSecurityProfile](../resources/ipsecurityprofile.md) collection||
|providerTenantSettings|[providerTenantSetting](../resources/providertenantsetting.md) collection||
|secureScoreControlProfiles|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection||
|secureScores|[secureScore](../resources/securescore.md) collection||
|securityActions|[securityAction](../resources/securityaction.md) collection||
|tiIndicators|[tiIndicator](../resources/tiindicator.md) collection||
|userSecurityProfiles|[userSecurityProfile](../resources/usersecurityprofile.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security",
  "id": "String (identifier)",
  "providerStatus": [
    {
      "@odata.type": "microsoft.graph.securityProviderStatus",
      "enabled": true,
      "endpoint": "String",
      "region": "String"
    }
  ]
}
```

