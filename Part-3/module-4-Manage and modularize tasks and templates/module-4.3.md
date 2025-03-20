# Exercise: Create and Manage Variable Groups in Azure DevOps

## Overview
In this exercise, you will learn how to create and manage Variable Groups in Azure DevOps. Variable groups allow you to store and reuse variables across multiple pipelines and stages, reducing redundancy and improving consistency.

## Steps to Create and Manage Variable Groups

### Step 1: Navigate to Variable Groups
1. Go to the **Parts Unlimited** project in Azure DevOps.
2. Click on **Pipelines** in the main menu.
3. Select **Library** under the Pipelines section.
4. You will see that there are no existing variable groups.

### Step 2: Create a Variable Group
1. Click **+ Variable Group** to create a new variable group.
2. Set the **Variable group name** to `Website Test Product Details`.

### Step 3: Add Variables to the Group
1. In the **Variables** section, click **+ Add** to add a new variable.
   - **Name:** ProductCode  
   - **Value:** REDPOLOXL  
2. Add another variable:
   - **Name:** Quantity  
   - **Value:** 12  
3. Add a third variable:
   - **Name:** SalesUnit  
   - **Value:** Each  

### Step 4: Save the Variable Group
1. Click **Save** to save the variable group.

### Step 5: Link Variable Group to a Release Pipeline
1. Go to **Pipelines > Releases** in the main menu.
2. Click **Edit** to open the release pipeline you are working on.
3. From the top menu, click **Variables**.
4. In the left-hand pane, click **Variable Groups**.
5. Click **Link variable group**.
6. In the **Link variable group** pane:
   - Select the `Website Test Product Details` variable group.
   - Set the **Variable group scope** to the following stages:
     - Development
     - Test Team A
     - Test Team B
   - Click **Link** to complete the process.

## Key Points
- **Variable Groups** allow you to reuse variables across multiple pipelines and stages.
- You can mark variables as **secret** to hide their values in logs.
- Variable groups can be linked to specific stages in a release pipeline.

https://learn.microsoft.com/en-us/training/modules/manage-modularize-tasks-templates/4-exercise-create-manage-variable-groups