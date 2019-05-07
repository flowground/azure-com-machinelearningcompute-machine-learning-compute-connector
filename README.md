# ![LOGO](logo.png) Machine Learning Compute Management Client **flow**ground Connector

## Description

A generated **flow**ground connector for the Machine Learning Compute Management Client API (version 2017-08-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/machinelearningcompute-machineLearningCompute/2017-08-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:38:19+03:00

## API Description

These APIs allow end users to operate on Azure Machine Learning Compute resources. They support the following operations:<ul><li>Create or update a cluster</li><li>Get a cluster</li><li>Patch a cluster</li><li>Delete a cluster</li><li>Get keys for a cluster</li><li>Check if updates are available for system services in a cluster</li><li>Update system services in a cluster</li><li>Get all clusters in a resource group</li><li>Get all clusters in a subscription</li></ul>

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets all available operations.

*Tags:* `MachineLearningComputeOperations`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.

### Gets the operationalization clusters in the specified subscription.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `$skiptoken` - _optional_ - Continuation token for pagination.

### Gets the clusters in the specified resource group.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `$skiptoken` - _optional_ - Continuation token for pagination.

### Deletes the specified cluster.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.
* `deleteAll` - _optional_ - If true, deletes all resources associated with this cluster.

### Gets the operationalization cluster resource view. Note that the credentials are not returned by this call. Call ListKeys to get them.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.

### The PATCH operation can be used to update only the tags for a cluster. Use PUT operation to update other properties.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.

### Create or update an operationalization cluster.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.

### Checks if updates are available for system services in the cluster.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.

### Gets the credentials for the specified cluster such as Storage, ACR and ACS credentials. This is a long running operation because it fetches keys from dependencies.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.

### Updates system services in a cluster.

*Tags:* `OperationalizationClusters`

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearningCompute resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - Name of the resource group in which the cluster is located.
* `clusterName` - _required_ - The name of the cluster.

## License

**flow**ground :- Telekom iPaaS / azure-com-machinelearningcompute-machine-learning-compute-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
