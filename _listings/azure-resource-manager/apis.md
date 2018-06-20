---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Azure Resource Manager
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API Resource Links Delete
  x-api-slug: azure-resource-manager-api
  description: Deletes a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{linkId}
  tags: Resource Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/linkid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/linkid-delete-openapi.md
- name: Azure Resource Manager API Resource Links Create Or Update
  x-api-slug: azure-resource-manager-api
  description: Creates or updates a resource link between the specified resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{linkId}
  tags: Resource Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/linkid-put-openapi.md
- name: Azure Resource Manager API Resource Links Get
  x-api-slug: azure-resource-manager-api
  description: Gets a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{linkId}
  tags: Resource Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/linkid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/linkid-get-openapi.md
- name: Azure Resource Manager API Resource Links List At Subscription
  x-api-slug: azure-resource-manager-api
  description: Gets all the linked resources for the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Resources/links
  tags: Resource Links At Subscription
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-openapi.md
- name: Azure Resource Manager API Resource Links List At Source Scope
  x-api-slug: azure-resource-manager-api
  description: Gets a list of resource links at and below the specified source scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Resources/links
  tags: Resource Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-openapi.md
- name: Azure Resource Manager API Creates or updates a management lock at the resource
    group level.
  x-api-slug: azure-resource-manager-api
  description: When you apply a lock at a parent scope, all child resources inherit
    the same lock. To create management locks, you must have access to Microsoft.Authorization/*
    or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
    and User Access Administrator are granted those actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Ss A Management Lock At Resource Group Level.
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlockslockname-put-openapi.md
- name: Azure Resource Manager API Deletes a management lock at the resource group
    level.
  x-api-slug: azure-resource-manager-api
  description: To delete management locks, you must have access to Microsoft.Authorization/*
    or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
    and User Access Administrator are granted those actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/locks/{lockName}
  tags: S A Management Lock At Resource Group Level.
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlockslockname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlockslockname-delete-openapi.md
- name: Azure Resource Manager API Management Locks Get At Resource Group Level
  x-api-slug: azure-resource-manager-api
  description: Gets a management lock at the resource group level.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks At Resource Group Level
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlockslockname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlockslockname-get-openapi.md
- name: Azure Resource Manager API Management Locks Create Or Update By Scope
  x-api-slug: azure-resource-manager-api
  description: Create or update a management lock by scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks Scope
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationlockslockname-put-openapi.md
- name: Azure Resource Manager API Management Locks Delete By Scope
  x-api-slug: azure-resource-manager-api
  description: Delete a management lock by scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks Scope
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationlockslockname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationlockslockname-delete-openapi.md
- name: Azure Resource Manager API Management Locks Get By Scope
  x-api-slug: azure-resource-manager-api
  description: Get a management lock by scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks Scope
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationlockslockname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationlockslockname-get-openapi.md
- name: Azure Resource Manager API Creates or updates a management lock at the resource
    level or any level below the resource.
  x-api-slug: azure-resource-manager-api
  description: When you apply a lock at a parent scope, all child resources inherit
    the same lock. To create management locks, you must have access to Microsoft.Authorization/*
    or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
    and User Access Administrator are granted those actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlockslockname-put-openapi.md
- name: Azure Resource Manager API Deletes the management lock of a resource or any
    level below the resource.
  x-api-slug: azure-resource-manager-api
  description: To delete management locks, you must have access to Microsoft.Authorization/*
    or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
    and User Access Administrator are granted those actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlockslockname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlockslockname-delete-openapi.md
- name: Azure Resource Manager API Management Locks Get At Resource Level
  x-api-slug: azure-resource-manager-api
  description: Get the management lock of a resource or any level below resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlockslockname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlockslockname-get-openapi.md
- name: Azure Resource Manager API Creates or updates a management lock at the subscription
    level.
  x-api-slug: azure-resource-manager-api
  description: When you apply a lock at a parent scope, all child resources inherit
    the same lock. To create management locks, you must have access to Microsoft.Authorization/*
    or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
    and User Access Administrator are granted those actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Ss A Management Lock At Subscription Level.
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlockslockname-put-openapi.md
- name: Azure Resource Manager API Deletes the management lock at the subscription
    level.
  x-api-slug: azure-resource-manager-api
  description: To delete management locks, you must have access to Microsoft.Authorization/*
    or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
    and User Access Administrator are granted those actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/locks/{lockName}
  tags: S Management Lock At Subscription Level.
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlockslockname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlockslockname-delete-openapi.md
- name: Azure Resource Manager API Management Locks Get At Subscription Level
  x-api-slug: azure-resource-manager-api
  description: Gets a management lock at the subscription level.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/locks/{lockName}
  tags: Management Locks At Subscription Level
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlockslockname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlockslockname-get-openapi.md
- name: Azure Resource Manager API Management Locks List At Resource Group Level
  x-api-slug: azure-resource-manager-api
  description: Gets all the management locks for a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/locks
  tags: Management Locks At Resource Group Level
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlocks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationlocks-get-openapi.md
- name: Azure Resource Manager API Management Locks List At Resource Level
  x-api-slug: azure-resource-manager-api
  description: Gets all the management locks for a resource or any level below resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/locks
  tags: Management Locks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlocks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationlocks-get-openapi.md
- name: Azure Resource Manager API Management Locks List At Subscription Level
  x-api-slug: azure-resource-manager-api
  description: Gets all the management locks for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/locks
  tags: Management Locks At Subscription Level
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlocks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationlocks-get-openapi.md
- name: Azure Resource Manager API Policy Assignments Delete
  x-api-slug: azure-resource-manager-api
  description: Deletes a policy assignment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-delete-openapi.md
- name: Azure Resource Manager API Creates a policy assignment.
  x-api-slug: azure-resource-manager-api
  description: Policy assignments are inherited by child resources. For example, when
    you apply a policy to a resource group that policy is assigned to all resources
    in the group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}
  tags: Policy Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-put-openapi.md
- name: Azure Resource Manager API Policy Assignments Get
  x-api-slug: azure-resource-manager-api
  description: Gets a policy assignment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-get-openapi.md
- name: Azure Resource Manager API Policy Assignments List For Resource Group
  x-api-slug: azure-resource-manager-api
  description: Gets policy assignments for the resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/policyAssignments
  tags: Policy Assignments For Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationpolicyassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationpolicyassignments-get-openapi.md
- name: Azure Resource Manager API Policy Assignments List For Resource
  x-api-slug: azure-resource-manager-api
  description: Gets policy assignments for a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/policyassignments
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationpolicyassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationpolicyassignments-get-openapi.md
- name: Azure Resource Manager API Policy Assignments List
  x-api-slug: azure-resource-manager-api
  description: Gets all the policy assignments for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policyassignments
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicyassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicyassignments-get-openapi.md
- name: Azure Resource Manager API Deletes a policy assignment by ID.
  x-api-slug: azure-resource-manager-api
  description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{policyAssignmentId}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/policyassignmentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/policyassignmentid-delete-openapi.md
- name: Azure Resource Manager API Creates a policy assignment by ID.
  x-api-slug: azure-resource-manager-api
  description: Policy assignments are inherited by child resources. For example, when
    you apply a policy to a resource group that policy is assigned to all resources
    in the group. When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{policyAssignmentId}
  tags: Policy Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/policyassignmentid-put-openapi.md
- name: Azure Resource Manager API Gets a policy assignment by ID.
  x-api-slug: azure-resource-manager-api
  description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{policyAssignmentId}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/policyassignmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/policyassignmentid-get-openapi.md
- name: Azure Resource Manager API Policy Definitions Create Or Update
  x-api-slug: azure-resource-manager-api
  description: Creates or updates a policy definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policydefinitions/{policyDefinitionName}
  tags: Policy Definitions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitionspolicydefinitionname-put-openapi.md
- name: Azure Resource Manager API Policy Definitions Delete
  x-api-slug: azure-resource-manager-api
  description: Deletes a policy definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policydefinitions/{policyDefinitionName}
  tags: Policy Definitions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitionspolicydefinitionname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitionspolicydefinitionname-delete-openapi.md
- name: Azure Resource Manager API Policy Definitions Get
  x-api-slug: azure-resource-manager-api
  description: Gets the policy definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policydefinitions/{policyDefinitionName}
  tags: Policy Definitions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitionspolicydefinitionname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitionspolicydefinitionname-get-openapi.md
- name: Azure Resource Manager API Policy Definitions List
  x-api-slug: azure-resource-manager-api
  description: Gets all the policy definitions for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policydefinitions
  tags: Policy Definitions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicydefinitions-get-openapi.md
- name: Azure Resource Manager API Deletes a deployment from the deployment history.
  x-api-slug: azure-resource-manager-api
  description: A template deployment that is currently running cannot be deleted.
    Deleting a template deployment removes the associated deployment operations. Deleting
    a template deployment does not affect the state of the resource group. This is
    an asynchronous operation that returns a status of 202 until the template deployment
    is successfully deleted. The Location response header contains the URI that is
    used to obtain the status of the process. While the process is running, a call
    to the URI in the Location header returns a status of 202. When the process finishes,
    the URI in the Location header returns a status of 204 on success. If the asynchronous
    request failed, the URI in the Location header returns an error-level status code.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}
  tags: Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-delete-openapi.md
- name: Azure Resource Manager API Deployments Check Existence
  x-api-slug: azure-resource-manager-api
  description: Checks whether the deployment exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}
  tags: Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-head-openapi.md
- name: Azure Resource Manager API Deploys resources to a resource group.
  x-api-slug: azure-resource-manager-api
  description: You can provide the template and parameters directly in the request
    or link to JSON files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}
  tags: Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-put-openapi.md
- name: Azure Resource Manager API Deployments Get
  x-api-slug: azure-resource-manager-api
  description: Gets a deployment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}
  tags: Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-get-openapi.md
- name: Azure Resource Manager API Cancels a currently running template deployment.
  x-api-slug: azure-resource-manager-api
  description: You can cancel a deployment only if the provisioningState is Accepted
    or Running. After the deployment is canceled, the provisioningState is set to
    Canceled. Canceling a template deployment stops the currently running template
    deployment and leaves the resource group partially deployed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}/cancel
  tags: Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnamecancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnamecancel-post-openapi.md
- name: Azure Resource Manager API Deployments Validate
  x-api-slug: azure-resource-manager-api
  description: Validates whether the specified template is syntactically correct and
    will be accepted by Azure Resource Manager..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}/validate
  tags: Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnamevalidate-post-openapi.md
- name: Azure Resource Manager API Deployments Export Template
  x-api-slug: azure-resource-manager-api
  description: Exports the template used for specified deployment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}/exportTemplate
  tags: Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnameexporttemplate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnameexporttemplate-post-openapi.md
- name: Azure Resource Manager API Deployments List
  x-api-slug: azure-resource-manager-api
  description: Get all the deployments for a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/
  tags: Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeployments-get-openapi.md
- name: Azure Resource Manager API Providers Unregister
  x-api-slug: azure-resource-manager-api
  description: Unregisters a subscription from a resource provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/{resourceProviderNamespace}/unregister
  tags: Providers Unregister
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersresourceprovidernamespaceunregister-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersresourceprovidernamespaceunregister-post-openapi.md
- name: Azure Resource Manager API Providers Register
  x-api-slug: azure-resource-manager-api
  description: Registers a subscription with a resource provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/{resourceProviderNamespace}/register
  tags: Providers Register
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersresourceprovidernamespaceregister-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersresourceprovidernamespaceregister-post-openapi.md
- name: Azure Resource Manager API Providers List
  x-api-slug: azure-resource-manager-api
  description: Gets all resource providers for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers
  tags: Providers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidproviders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidproviders-get-openapi.md
- name: Azure Resource Manager API Providers Get
  x-api-slug: azure-resource-manager-api
  description: Gets the specified resource provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/{resourceProviderNamespace}
  tags: Providers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersresourceprovidernamespace-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersresourceprovidernamespace-get-openapi.md
- name: Azure Resource Manager API Resource Groups List Resources
  x-api-slug: azure-resource-manager-api
  description: Get all the resources for a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/resources
  tags: Resource Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get-openapi.md
- name: Azure Resource Manager API Resource Groups Check Existence
  x-api-slug: azure-resource-manager-api
  description: Checks whether a resource group exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: Resource Groups Existence
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-openapi.md
- name: Azure Resource Manager API Resource Groups Create Or Update
  x-api-slug: azure-resource-manager-api
  description: Creates a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: Resource Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-put-openapi.md
- name: Azure Resource Manager API Deletes a resource group.
  x-api-slug: azure-resource-manager-api
  description: When you delete a resource group, all of its resources are also deleted.
    Deleting a resource group deletes all of its template deployments and currently
    stored operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: S A Resource Group.
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-delete-openapi.md
- name: Azure Resource Manager API Resource Groups Get
  x-api-slug: azure-resource-manager-api
  description: Gets a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: Resource Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-get-openapi.md
- name: Azure Resource Manager API Updates a resource group.
  x-api-slug: azure-resource-manager-api
  description: Resource groups can be updated through a simple PATCH operation to
    a group address. The format of the request is the same as that for creating a
    resource group. If a field is unspecified, the current value is retained.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: S A Resource Group.
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-patch-openapi.md
- name: Azure Resource Manager API Resource Groups Export Template
  x-api-slug: azure-resource-manager-api
  description: Captures the specified resource group as a template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/exportTemplate
  tags: Resource Groups Export Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post-openapi.md
- name: Azure Resource Manager API Resource Groups List
  x-api-slug: azure-resource-manager-api
  description: Gets all the resource groups for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups
  tags: Resource Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroups-get-openapi.md
- name: Azure Resource Manager API Moves resources from one resource group to another
    resource group.
  x-api-slug: azure-resource-manager-api
  description: The resources to move must be in the same source resource group. The
    target resource group may be in a different subscription. When moving resources,
    both the source group and the target group are locked for the duration of the
    operation. Write and delete operations are blocked on the groups until the move
    completes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{sourceResourceGroupName}/moveResources
  tags: Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupssourceresourcegroupnamemoveresources-post-openapi.md
- name: Azure Resource Manager API Resources List
  x-api-slug: azure-resource-manager-api
  description: Get all the resources in a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resources
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresources-get-openapi.md
- name: Azure Resource Manager API Resources Check Existence
  x-api-slug: azure-resource-manager-api
  description: Checks whether a resource exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head-openapi.md
- name: Azure Resource Manager API Resources Delete
  x-api-slug: azure-resource-manager-api
  description: Deletes a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete-openapi.md
- name: Azure Resource Manager API Resources Create Or Update
  x-api-slug: azure-resource-manager-api
  description: Creates a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}
  tags: Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-put-openapi.md
- name: Azure Resource Manager API Resources Get
  x-api-slug: azure-resource-manager-api
  description: Gets a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-get-openapi.md
- name: Azure Resource Manager API Resources Check Existence By Id
  x-api-slug: azure-resource-manager-api
  description: Checks by ID whether a resource exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{resourceId}
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-head-openapi.md
- name: Azure Resource Manager API Resources Delete By Id
  x-api-slug: azure-resource-manager-api
  description: Deletes a resource by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{resourceId}
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-delete-openapi.md
- name: Azure Resource Manager API Resources Create Or Update By Id
  x-api-slug: azure-resource-manager-api
  description: Create a resource by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{resourceId}
  tags: Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-put-openapi.md
- name: Azure Resource Manager API Resources Get By Id
  x-api-slug: azure-resource-manager-api
  description: Gets a resource by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{resourceId}
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/resourceid-get-openapi.md
- name: Azure Resource Manager API Tags Delete Value
  x-api-slug: azure-resource-manager-api
  description: Deletes a tag value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}/tagValues/{tagValue}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-delete-openapi.md
- name: Azure Resource Manager API Tags Create Or Update Value
  x-api-slug: azure-resource-manager-api
  description: Creates a tag value. The name of the tag must already exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}/tagValues/{tagValue}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-put-openapi.md
- name: Azure Resource Manager API Creates a tag in the subscription.
  x-api-slug: azure-resource-manager-api
  description: The tag name can have a maximum of 512 characters and is case insensitive.
    Tag names created by Azure have prefixes of microsoft, azure, or windows. You
    cannot create tags with one of these prefixes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-put-openapi.md
- name: Azure Resource Manager API Deletes a tag from the subscription.
  x-api-slug: azure-resource-manager-api
  description: You must remove all values from a resource tag before you can delete
    it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-delete-openapi.md
- name: Azure Resource Manager API Tags List
  x-api-slug: azure-resource-manager-api
  description: Gets the names and values of all resource tags that are defined in
    a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnames-get-openapi.md
- name: Azure Resource Manager API Deployment Operations Get
  x-api-slug: azure-resource-manager-api
  description: Gets a deployments operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/deployments/{deploymentName}/operations/{operationId}
  tags: Deployment Operations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnamedeploymentsdeploymentnameoperationsoperationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnamedeploymentsdeploymentnameoperationsoperationid-get-openapi.md
- name: Azure Resource Manager API Deployment Operations List
  x-api-slug: azure-resource-manager-api
  description: Gets all deployments operations for a deployment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/deployments/{deploymentName}/operations
  tags: Deployment Operations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnamedeploymentsdeploymentnameoperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnamedeploymentsdeploymentnameoperations-get-openapi.md
- name: Azure Resource Manager API Gets all available geo-locations.
  x-api-slug: azure-resource-manager-api
  description: This operation provides all the locations that are available for resource
    providers; however, each resource provider may support a subset of this list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/locations
  tags: S All Available Geo-locations.
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidlocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionidlocations-get-openapi.md
- name: Azure Resource Manager API Subscriptions Get
  x-api-slug: azure-resource-manager-api
  description: Gets details about a specified subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptionssubscriptionid-get-openapi.md
- name: Azure Resource Manager API Subscriptions List
  x-api-slug: azure-resource-manager-api
  description: Gets all subscriptions for a tenant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/subscriptions-get-openapi.md
- name: Azure Resource Manager API Tenants List
  x-api-slug: azure-resource-manager-api
  description: Gets the tenants for your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////tenants
  tags: Tenants
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/tenants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/tenants-get-openapi.md
- name: Azure Resource Manager API
  x-api-slug: azure-resource-manager-api
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions. You organize related resources in resource groups, and
    deploy your resources with JSON templates. For an introduction to deploying and
    managing resources with Resource Manager, see Azure Resource Manager overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Azure Resource Manager
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-resource-manager/master/_listings/azure-resource-manager/openapi.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---