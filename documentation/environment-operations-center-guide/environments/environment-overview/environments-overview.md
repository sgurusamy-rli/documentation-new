---
keywords:
title: Environments Overview
description: Overview of the Environments home screen user interface
---
# Environments Overview

This guide provides an overview of the *Environments* home screen and its features. To navigate to the *Environments* home screen, select **Environments** in the left navigation.

![image description](images/select-envs.png)

The *Environments* home screen provides an overview of all your organization's available environments. Each environment is displayed, including its name, type, status, creation date, version, and number of nodes.

Two environment display views are available, either list- or grid-view. In the list-view, environments are organized by row with the associated environment details contained in the row.

![image description](images/envs-list-view.png)

In the grid-view, environments are organized in a card format with associated details for an environment contained within the card.

![image description](images/envs-grid-view.png)

Each environment has its own **Options** menu (**...**) that allows you to perform various operations on the selected environment. In the list-view, the options menu is located at the end of an environment row.

![image description](images/options-list.png)

In the grid-view, the options menu is located in the upper corner of an environment card.

![image description](images/options-grid.png)

A **Search For** bar at the top of the *Environments* screen can be used to filter the listed environments. Enter an environment name, specific characters, or words in the space provided to quickly filter through the environments.

![image description](images/search-to-filter.png)

A refresh button is located in the upper right corner of the *Environments* screen. Select the refresh icon to pull up to date information about the environments.

![image description](images/refresh-envs.png)

## Environment details

To access further details about an environment, select the name of the environment you wish to view. 

![image description](images/env-details.png)

This brings you to the environment's *Overview* screen, where you can view further information about a given environment, such as node status or connections, and perform monitoring and updating actions.

[!note] To learn more about the environment *Overview* features, review the [environment details](environments/environment-details/environment-details-ui.md) guide.

![image description](images/detailed-view.png)
  
## Environment type

The environment **Type** is listed below the environment name and indicates whether the environment is configured as a "Production or "Non-production" environment. "Production" environments are for production purposes, and "Non-production" environments are for development and testing.

[!note] The number of production and non-production environments available will differ depending on your organization's selected tier. Please contact your RadiantOne account representative to adjust your tier if you require additional environments.

![image description](images/env-type.png)

## Environment status

The environment **Status** indicates the current state of the environment. Statuses automatically change as operations are performed on an environment or if any errors have occurred. Environment statuses include:

- Operational: Indicates all FID and Zookeeper nodes are running.
- Warning: There are nodes not running, but the minimum number of nodes required for an environment to operate are running.
- Outage: The minimum number of nodes required for an environment to operate are not running.
- Update failed: An attempt to update the environment failed.
- Creation failed: An attempt to create a new environment failed.
- Import failed: An attempt to import a configuration file failed.
- Updating: The environment is currently updating (this can take up to 1 hour).
- Creating: The environment is currently being created (this can take up to 1 hour).

![image description](images/env-status.png)

## Environment creation date

The **Creation Date** indicates the date and time when the environment was created.

![image description](images/creation-date.png)

## Environment version

**Version** indicates the current version of the environment. The version number is set by the environment administrator during environment setup. If the environment version number no longer matches the current available version of Environment Operations Center, an "Update Now" notification is displayed next to the version number prompting you to update the environment. 

To learn more about updating an environment, review the [update an environment](update-an-environment.md) guide.

![image description](images/version.png)

## Environment nodes

**Nodes** indicates the number of nodes in the environment. The number of nodes is set by the environment administrator during environment setup. An environment Administrator can increase or decrease the number of nodes in an environment at any time.

To learn more about adjusting the number of nodes in an environment, see the [update and monitor nodes](../environment-details/node-details.md) guide.

![images description](images/nodes.png)

## Options Menu

To view a list of operations that can be performed on a given environment, select the ellipsis (**...**) in the environment row or card to expand the **Options** menu. Options include:

- **View Details**: takes you to an environment's *Overview* screen where you can view further details about the environment. To learn more about the environment *Overview*, review the [environment overview guide](../environment-details/environment-details-ui.md).
- **Update**: opens the dialog to begin the update an environment workflow. This option will only be available in the menu dropdown if an update is available. For more information on updating an environment, review the [update an environment](update-an-environment.md) guide.
- **Adjust Scale**: opens the *Adjust Environment Scale* dialog, where you can increase or decrease the number of nodes in the environments. For more information on updating nodes, see the [update and monitor nodes](../environment-details/node-details.md) guide.
- **View logs**: takes you to an environment's *Logs* screen where you can view log files for a given date range. To learn how to review logs, visit the environment details [logs](../environment-details/environment-logs.md) guide.
- **Delete**: opens the dialog to being the workflow to delete an environment. For information on deleting an environment, review the [delete and environment](delete-an-environment.md) guide.

![image description](images/options-menu.png)

## New environment

The **New Environment** button allows you to quickly start creating a new environment from the home screen. For details on how to create a new environment, review the guide on [creating a new environment](create-an-environment.md).

![image description](images/new-env.png)

## Access Permissions

Depending on your role, your administrator may set your access permissions to read-only for certain environments. If you have read-only access:

- You will not be able to create new environments and the **New Environment** button will be deactivated.
- Certain environments will be hidden if you have not been assigned either read-only or editing permissions.
- You will not be able to edit or update the environments that you have read-only access to and the **Options** menu (**...**) will no longer be visible next to the environment. You can still view the details for these environments by selecting the environment name to navigate to their respective "Overview" screens.
- An administrator can assign editing permission to you for specific environments. This allows you to edit, update, or delete the environments they have specified, while others remain hidden or read-only.

## Next Steps

After reading this guide you should have an understanding of how to navigate the *Environments* home screen and its main features. To begin setting up a new environment, review the documentation on [creating a new environment](create-an-environment.md).