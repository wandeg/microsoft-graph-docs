### Identity and access (Azure AD)

| **Change type** | **Version** | **Description** |
|:---|:---|:---|
|Addition|beta|Added the `ValueAddOnly` member to the **attributeFlowType** enumeration|
|Addition|beta|Added the `AttributeAddOnly` member to the **attributeFlowType** enumeration|
|Addition|beta|Added the `SkipOutOfScopeDeletions` member to the **synchronizationSecret** enumeration|
|Addition|beta|Added the `Oauth2AuthorizationCode` member to the **synchronizationSecret** enumeration|
|Addition|beta|Added the `Oauth2RedirectUri` member to the **synchronizationSecret** enumeration|
|Addition|beta|Added the `ApplicationTemplateIdentifier` member to the **synchronizationSecret** enumeration|
|Addition|beta|Added the `IngestionInterrupted` member to the **quarantineReason** enumeration|
|Addition|beta|Added the `Paused` member to the **synchronizationScheduleState** enumeration|
|Deletion|beta|Removed the **provisioningTaskIdentifier** property from [synchronizationSchema](/graph/api/resources/synchronization-synchronizationSchema?view=graph-rest-beta) resource|
|Deletion|beta|Removed the **apply** method from the [synchronizationJob](/graph/api/resources/synchronization-synchronizationJob?view=graph-rest-beta) resource|
|Deletion|beta|Removed the **discover** method from the [directoryDefinition](/graph/api/resources/synchronization-directoryDefinition?view=graph-rest-beta) resource|
