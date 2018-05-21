---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 0
info:
  title: Azure Resource Manager API Resources Delete
  description: Deletes a resource.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policydefinitions:
    get:
      summary: Policy Definitions List
      description: Gets all the policy definitions for a subscription.
      operationId: PolicyDefinitions_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftauthorizationpolicydefinitions-get
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
      - Policy Definitions
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}:
    delete:
      summary: Deletes a deployment from the deployment history.
      description: A template deployment that is currently running cannot be deleted.
        Deleting a template deployment removes the associated deployment operations.
        Deleting a template deployment does not affect the state of the resource group.
        This is an asynchronous operation that returns a status of 202 until the template
        deployment is successfully deleted. The Location response header contains
        the URI that is used to obtain the status of the process. While the process
        is running, a call to the URI in the Location header returns a status of 202.
        When the process finishes, the URI in the Location header returns a status
        of 204 on success. If the asynchronous request failed, the URI in the Location
        header returns an error-level status code.
      operationId: Deployments_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentname-delete
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment to delete
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group with the deployment to delete
      responses:
        200:
          description: OK
      tags:
      - Deployments
    head:
      summary: Deployments Check Existence
      description: Checks whether the deployment exists.
      operationId: Deployments_CheckExistence
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentname-head
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment to check
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group with the deployment to check
      responses:
        200:
          description: OK
      tags:
      - Deployments
    put:
      summary: Deploys resources to a resource group.
      description: You can provide the template and parameters directly in the request
        or link to JSON files.
      operationId: Deployments_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentname-put
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Additional parameters supplied to the operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to deploy the resources to
      responses:
        200:
          description: OK
      tags:
      - Deployments
    get:
      summary: Deployments Get
      description: Gets a deployment.
      operationId: Deployments_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentname-get
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment to get
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Deployments
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}/cancel
  : post:
      summary: Cancels a currently running template deployment.
      description: You can cancel a deployment only if the provisioningState is Accepted
        or Running. After the deployment is canceled, the provisioningState is set
        to Canceled. Canceling a template deployment stops the currently running template
        deployment and leaves the resource group partially deployed.
      operationId: Deployments_Cancel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentnamecancel-post
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment to cancel
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Deployments
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}/validate
  : post:
      summary: Deployments Validate
      description: Validates whether the specified template is syntactically correct
        and will be accepted by Azure Resource Manager..
      operationId: Deployments_Validate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentnamevalidate-post
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters to validate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group the template will be deployed
          to
      responses:
        200:
          description: OK
      tags:
      - Deployments
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}/exportTemplate
  : post:
      summary: Deployments Export Template
      description: Exports the template used for specified deployment.
      operationId: Deployments_ExportTemplate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeploymentsdeploymentnameexporttemplate-post
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment from which to get the template
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/:
    get:
      summary: Deployments List
      description: Get all the deployments for a resource group.
      operationId: Deployments_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftresourcesdeployments-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to get
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group with the deployments to get
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /subscriptions/{subscriptionId}/providers/{resourceProviderNamespace}/unregister:
    post:
      summary: Providers Unregister
      description: Unregisters a subscription from a resource provider.
      operationId: Providers_Unregister
      x-api-path-slug: subscriptionssubscriptionidprovidersresourceprovidernamespaceunregister-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider to unregister
      responses:
        200:
          description: OK
      tags:
      - Providers Unregister
  /subscriptions/{subscriptionId}/providers/{resourceProviderNamespace}/register:
    post:
      summary: Providers Register
      description: Registers a subscription with a resource provider.
      operationId: Providers_Register
      x-api-path-slug: subscriptionssubscriptionidprovidersresourceprovidernamespaceregister-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider to register
      responses:
        200:
          description: OK
      tags:
      - Providers Register
  /subscriptions/{subscriptionId}/providers:
    get:
      summary: Providers List
      description: Gets all resource providers for a subscription.
      operationId: Providers_List
      x-api-path-slug: subscriptionssubscriptionidproviders-get
      parameters:
      - in: query
        name: $expand
        description: The properties to include in the results
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Providers
  /subscriptions/{subscriptionId}/providers/{resourceProviderNamespace}:
    get:
      summary: Providers Get
      description: Gets the specified resource provider.
      operationId: Providers_Get
      x-api-path-slug: subscriptionssubscriptionidprovidersresourceprovidernamespace-get
      parameters:
      - in: query
        name: $expand
        description: The $expand query parameter
      - in: query
        name: No Name
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      responses:
        200:
          description: OK
      tags:
      - Providers
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/resources:
    get:
      summary: Resource Groups List Resources
      description: Get all the resources for a resource group.
      operationId: ResourceGroups_ListResources
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get
      parameters:
      - in: query
        name: $expand
        description: The $expand query parameter
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group with the resources to get
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}:
    head:
      summary: Resource Groups Check Existence
      description: Checks whether a resource group exists.
      operationId: ResourceGroups_CheckExistence
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-head
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group to check
      responses:
        200:
          description: OK
      tags:
      - Resource Groups Existence
    put:
      summary: Resource Groups Create Or Update
      description: Creates a resource group.
      operationId: ResourceGroups_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the create or update a resource group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to create or update
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
    delete:
      summary: Deletes a resource group.
      description: When you delete a resource group, all of its resources are also
        deleted. Deleting a resource group deletes all of its template deployments
        and currently stored operations.
      operationId: ResourceGroups_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group to delete
      responses:
        200:
          description: OK
      tags:
      - S A Resource Group.
    get:
      summary: Resource Groups Get
      description: Gets a resource group.
      operationId: ResourceGroups_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group to get
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
    patch:
      summary: Updates a resource group.
      description: Resource groups can be updated through a simple PATCH operation
        to a group address. The format of the request is the same as that for creating
        a resource group. If a field is unspecified, the current value is retained.
      operationId: ResourceGroups_Patch
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to update a resource group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to update
      responses:
        200:
          description: OK
      tags:
      - S A Resource Group.
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/exportTemplate:
    post:
      summary: Resource Groups Export Template
      description: Captures the specified resource group as a template.
      operationId: ResourceGroups_ExportTemplate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for exporting the template
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to export as a template
      responses:
        200:
          description: OK
      tags:
      - Resource Groups Export Template
  /subscriptions/{subscriptionId}/resourcegroups:
    get:
      summary: Resource Groups List
      description: Gets all the resource groups for a subscription.
      operationId: ResourceGroups_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroups-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
  /subscriptions/{subscriptionId}/resourceGroups/{sourceResourceGroupName}/moveResources:
    post:
      summary: Moves resources from one resource group to another resource group.
      description: The resources to move must be in the same source resource group.
        The target resource group may be in a different subscription. When moving
        resources, both the source group and the target group are locked for the duration
        of the operation. Write and delete operations are blocked on the groups until
        the move completes.
      operationId: Resources_MoveResources
      x-api-path-slug: subscriptionssubscriptionidresourcegroupssourceresourcegroupnamemoveresources-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for moving resources
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: sourceResourceGroupName
        description: The name of the resource group containing the rsources to move
      responses:
        200:
          description: OK
      tags:
      - Resources
  /subscriptions/{subscriptionId}/resources:
    get:
      summary: Resources List
      description: Get all the resources in a subscription.
      operationId: Resources_List
      x-api-path-slug: subscriptionssubscriptionidresources-get
      parameters:
      - in: query
        name: $expand
        description: The $expand query parameter
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resources
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}
  : head:
      summary: Resources Check Existence
      description: Checks whether a resource exists.
      operationId: Resources_CheckExistence
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the resource to check
      - in: path
        name: resourceName
        description: The name of the resource to check whether it exists
      - in: path
        name: resourceProviderNamespace
        description: The resource provider of the resource to check
      - in: path
        name: resourceType
        description: The resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
    delete:
      summary: Resources Delete
      description: Deletes a resource.
      operationId: Resources_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the resource to
          delete
      - in: path
        name: resourceName
        description: The name of the resource to delete
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
      - Resources
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