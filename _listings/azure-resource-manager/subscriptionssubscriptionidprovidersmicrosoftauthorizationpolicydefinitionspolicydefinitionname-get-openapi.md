---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 0
info:
  title: Azure Resource Manager API Policy Definitions Get
  description: Gets the policy definition.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{linkId}:
    delete:
      summary: Resource Links Delete
      description: Deletes a resource link with the specified ID.
      operationId: ResourceLinks_Delete
      x-api-path-slug: linkid-delete
      parameters:
      - in: path
        name: linkId
        description: The fully qualified ID of the resource link
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Links
    put:
      summary: Resource Links Create Or Update
      description: Creates or updates a resource link between the specified resources.
      operationId: ResourceLinks_CreateOrUpdate
      x-api-path-slug: linkid-put
      parameters:
      - in: path
        name: linkId
        description: The fully qualified ID of the resource link
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for creating or updating a resource link
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Resource Links
    get:
      summary: Resource Links Get
      description: Gets a resource link with the specified ID.
      operationId: ResourceLinks_Get
      x-api-path-slug: linkid-get
      parameters:
      - in: path
        name: linkId
        description: The fully qualified Id of the resource link
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Links
  /subscriptions/{subscriptionId}/providers/Microsoft.Resources/links:
    get:
      summary: Resource Links List At Subscription
      description: Gets all the linked resources for the subscription.
      operationId: ResourceLinks_ListAtSubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftresourceslinks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the list resource links operation
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Links At Subscription
  /{scope}/providers/Microsoft.Resources/links:
    get:
      summary: Resource Links List At Source Scope
      description: Gets a list of resource links at and below the specified source
        scope.
      operationId: ResourceLinks_ListAtSourceScope
      x-api-path-slug: scopeprovidersmicrosoftresourceslinks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply when getting resource links
      - in: query
        name: No Name
      - in: path
        name: scope
        description: The fully qualified ID of the scope for getting the resource
          links
      responses:
        200:
          description: OK
      tags:
      - Resource Links
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/locks/{lockName}:
    put:
      summary: Creates or updates a management lock at the resource group level.
      description: When you apply a lock at a parent scope, all child resources inherit
        the same lock. To create management locks, you must have access to Microsoft.Authorization/*
        or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
        and User Access Administrator are granted those actions.
      operationId: ManagementLocks_CreateOrUpdateAtResourceGroupLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftauthorizationlockslockname-put
      parameters:
      - in: path
        name: lockName
        description: The lock name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The management lock parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to lock
      responses:
        200:
          description: OK
      tags:
      - Ss A Management Lock At Resource Group Level.
    delete:
      summary: Deletes a management lock at the resource group level.
      description: To delete management locks, you must have access to Microsoft.Authorization/*
        or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
        and User Access Administrator are granted those actions.
      operationId: ManagementLocks_DeleteAtResourceGroupLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftauthorizationlockslockname-delete
      parameters:
      - in: path
        name: lockName
        description: The name of lock to delete
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the lock
      responses:
        200:
          description: OK
      tags:
      - S A Management Lock At Resource Group Level.
    get:
      summary: Management Locks Get At Resource Group Level
      description: Gets a management lock at the resource group level.
      operationId: ManagementLocks_GetAtResourceGroupLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftauthorizationlockslockname-get
      parameters:
      - in: path
        name: lockName
        description: The name of the lock to get
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the locked resource group
      responses:
        200:
          description: OK
      tags:
      - Management Locks At Resource Group Level
  /{scope}/providers/Microsoft.Authorization/locks/{lockName}:
    put:
      summary: Management Locks Create Or Update By Scope
      description: Create or update a management lock by scope.
      operationId: ManagementLocks_CreateOrUpdateByScope
      x-api-path-slug: scopeprovidersmicrosoftauthorizationlockslockname-put
      parameters:
      - in: path
        name: lockName
        description: The name of lock
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create or update management lock parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: scope
        description: The scope for the lock
      responses:
        200:
          description: OK
      tags:
      - Management Locks Scope
    delete:
      summary: Management Locks Delete By Scope
      description: Delete a management lock by scope.
      operationId: ManagementLocks_DeleteByScope
      x-api-path-slug: scopeprovidersmicrosoftauthorizationlockslockname-delete
      parameters:
      - in: path
        name: lockName
        description: The name of lock
      - in: query
        name: No Name
      - in: path
        name: scope
        description: The scope for the lock
      responses:
        200:
          description: OK
      tags:
      - Management Locks Scope
    get:
      summary: Management Locks Get By Scope
      description: Get a management lock by scope.
      operationId: ManagementLocks_GetByScope
      x-api-path-slug: scopeprovidersmicrosoftauthorizationlockslockname-get
      parameters:
      - in: path
        name: lockName
        description: The name of lock
      - in: query
        name: No Name
      - in: path
        name: scope
        description: The scope for the lock
      responses:
        200:
          description: OK
      tags:
      - Management Locks Scope
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/locks/{lockName}
  : put:
      summary: Creates or updates a management lock at the resource level or any level
        below the resource.
      description: When you apply a lock at a parent scope, all child resources inherit
        the same lock. To create management locks, you must have access to Microsoft.Authorization/*
        or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
        and User Access Administrator are granted those actions.
      operationId: ManagementLocks_CreateOrUpdateAtResourceLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoftauthorizationlockslockname-put
      parameters:
      - in: path
        name: lockName
        description: The name of lock
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for creating or updating a  management lock
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the resource to lock
      - in: path
        name: resourceName
        description: The name of the resource to lock
      - in: path
        name: resourceProviderNamespace
        description: The resource provider namespace of the resource to lock
      - in: path
        name: resourceType
        description: The resource type of the resource to lock
      responses:
        200:
          description: OK
      tags:
      - Management Locks
    delete:
      summary: Deletes the management lock of a resource or any level below the resource.
      description: To delete management locks, you must have access to Microsoft.Authorization/*
        or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
        and User Access Administrator are granted those actions.
      operationId: ManagementLocks_DeleteAtResourceLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoftauthorizationlockslockname-delete
      parameters:
      - in: path
        name: lockName
        description: The name of the lock to delete
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the resource with the
          lock to delete
      - in: path
        name: resourceName
        description: The name of the resource with the lock to delete
      - in: path
        name: resourceProviderNamespace
        description: The resource provider namespace of the resource with the lock
          to delete
      - in: path
        name: resourceType
        description: The resource type of the resource with the lock to delete
      responses:
        200:
          description: OK
      tags:
      - Management Locks
    get:
      summary: Management Locks Get At Resource Level
      description: Get the management lock of a resource or any level below resource.
      operationId: ManagementLocks_GetAtResourceLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoftauthorizationlockslockname-get
      parameters:
      - in: path
        name: lockName
        description: The name of lock
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: An extra path parameter needed in some services, like SQL Databases
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: resourceName
        description: The name of the resource
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      - in: path
        name: resourceType
        description: The type of the resource
      responses:
        200:
          description: OK
      tags:
      - Management Locks
  /subscriptions/{subscriptionId}/providers/Microsoft.Authorization/locks/{lockName}:
    put:
      summary: Creates or updates a management lock at the subscription level.
      description: When you apply a lock at a parent scope, all child resources inherit
        the same lock. To create management locks, you must have access to Microsoft.Authorization/*
        or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
        and User Access Administrator are granted those actions.
      operationId: ManagementLocks_CreateOrUpdateAtSubscriptionLevel
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationlockslockname-put
      parameters:
      - in: path
        name: lockName
        description: The name of lock
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The management lock parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ss A Management Lock At Subscription Level.
    delete:
      summary: Deletes the management lock at the subscription level.
      description: To delete management locks, you must have access to Microsoft.Authorization/*
        or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner
        and User Access Administrator are granted those actions.
      operationId: ManagementLocks_DeleteAtSubscriptionLevel
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationlockslockname-delete
      parameters:
      - in: path
        name: lockName
        description: The name of lock to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - S Management Lock At Subscription Level.
    get:
      summary: Management Locks Get At Subscription Level
      description: Gets a management lock at the subscription level.
      operationId: ManagementLocks_GetAtSubscriptionLevel
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationlockslockname-get
      parameters:
      - in: path
        name: lockName
        description: The name of the lock to get
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Management Locks At Subscription Level
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/locks:
    get:
      summary: Management Locks List At Resource Group Level
      description: Gets all the management locks for a resource group.
      operationId: ManagementLocks_ListAtResourceGroupLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftauthorizationlocks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the locks to get
      responses:
        200:
          description: OK
      tags:
      - Management Locks At Resource Group Level
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/locks
  : get:
      summary: Management Locks List At Resource Level
      description: Gets all the management locks for a resource or any level below
        resource.
      operationId: ManagementLocks_ListAtResourceLevel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoftauthorizationlocks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the locked resource
      - in: path
        name: resourceName
        description: The name of the locked resource
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      - in: path
        name: resourceType
        description: The resource type of the locked resource
      responses:
        200:
          description: OK
      tags:
      - Management Locks
  /subscriptions/{subscriptionId}/providers/Microsoft.Authorization/locks:
    get:
      summary: Management Locks List At Subscription Level
      description: Gets all the management locks for a subscription.
      operationId: ManagementLocks_ListAtSubscriptionLevel
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationlocks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Management Locks At Subscription Level
  /{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}:
    delete:
      summary: Policy Assignments Delete
      description: Deletes a policy assignment.
      operationId: PolicyAssignments_Delete
      x-api-path-slug: scopeprovidersmicrosoftauthorizationpolicyassignmentspolicyassignmentname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policyAssignmentName
        description: The name of the policy assignment to delete
      - in: path
        name: scope
        description: The scope of the policy assignment
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
    put:
      summary: Creates a policy assignment.
      description: Policy assignments are inherited by child resources. For example,
        when you apply a policy to a resource group that policy is assigned to all
        resources in the group.
      operationId: PolicyAssignments_Create
      x-api-path-slug: scopeprovidersmicrosoftauthorizationpolicyassignmentspolicyassignmentname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for the policy assignment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policyAssignmentName
        description: The name of the policy assignment
      - in: path
        name: scope
        description: The scope of the policy assignment
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
    get:
      summary: Policy Assignments Get
      description: Gets a policy assignment.
      operationId: PolicyAssignments_Get
      x-api-path-slug: scopeprovidersmicrosoftauthorizationpolicyassignmentspolicyassignmentname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policyAssignmentName
        description: The name of the policy assignment to get
      - in: path
        name: scope
        description: The scope of the policy assignment
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/policyAssignments:
    get:
      summary: Policy Assignments List For Resource Group
      description: Gets policy assignments for the resource group.
      operationId: PolicyAssignments_ListForResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftauthorizationpolicyassignments-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains policy assignments
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments For Resource Group
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/policyassignments
  : get:
      summary: Policy Assignments List For Resource
      description: Gets policy assignments for a resource.
      operationId: PolicyAssignments_ListForResource
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoftauthorizationpolicyassignments-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource path
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the resource
      - in: path
        name: resourceName
        description: The name of the resource with policy assignments
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      - in: path
        name: resourceType
        description: The resource type
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
  /subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policyassignments:
    get:
      summary: Policy Assignments List
      description: Gets all the policy assignments for a subscription.
      operationId: PolicyAssignments_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationpolicyassignments-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
  /{policyAssignmentId}:
    delete:
      summary: Deletes a policy assignment by ID.
      description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
        for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
        for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
        for resources.
      operationId: PolicyAssignments_DeleteById
      x-api-path-slug: policyassignmentid-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policyAssignmentId
        description: The ID of the policy assignment to delete
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
    put:
      summary: Creates a policy assignment by ID.
      description: Policy assignments are inherited by child resources. For example,
        when you apply a policy to a resource group that policy is assigned to all
        resources in the group. When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
        for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
        for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
        for resources.
      operationId: PolicyAssignments_CreateById
      x-api-path-slug: policyassignmentid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for policy assignment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policyAssignmentId
        description: The ID of the policy assignment to create
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
    get:
      summary: Gets a policy assignment by ID.
      description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
        for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
        for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
        for resources.
      operationId: PolicyAssignments_GetById
      x-api-path-slug: policyassignmentid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policyAssignmentId
        description: The ID of the policy assignment to get
      responses:
        200:
          description: OK
      tags:
      - Policy Assignments
  /subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policydefinitions/{policyDefinitionName}:
    put:
      summary: Policy Definitions Create Or Update
      description: Creates or updates a policy definition.
      operationId: PolicyDefinitions_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationpolicydefinitionspolicydefinitionname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The policy definition properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policyDefinitionName
        description: The name of the policy definition to create
      responses:
        200:
          description: OK
      tags:
      - Policy Definitions
    delete:
      summary: Policy Definitions Delete
      description: Deletes a policy definition.
      operationId: PolicyDefinitions_Delete
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationpolicydefinitionspolicydefinitionname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policyDefinitionName
        description: The name of the policy definition to delete
      responses:
        200:
          description: OK
      tags:
      - Policy Definitions
    get:
      summary: Policy Definitions Get
      description: Gets the policy definition.
      operationId: PolicyDefinitions_Get
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationpolicydefinitionspolicydefinitionname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policyDefinitionName
        description: The name of the policy definition to get
      responses:
        200:
          description: OK
      tags:
      - Policy Definitions
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---