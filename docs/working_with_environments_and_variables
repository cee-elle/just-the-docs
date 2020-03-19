---
layout: default
title: Working With Environments & Variables
nav_order: 4
---

# Working with Environments & Variables
---

### Understanding Variables
A variable can be used as a reference tool and be defined with a specific value that a user sets. This tool can be useful when the variable exists in different places and may be changed at one place through the usage of a global variable. Therefore, this allows user changes to be more efficient and readable. 

### Understanding Environments 
An environment allows for collections and requests to be run against different data sets. You can have different environments meant for testing, development, and production that will need different data sets to be passed. In this application, environments are made up of key-value pairs of variables, and each variable represents its key. You may access it by referencing the variable. Let’s get started by creating your first environment.

For the example below, we will be taking sampel data from this website: https://reqres.in. On the site, there are a list of fake GET, POST, PUT, DELETE requests that can be made. The second column shows how to mock your request, and the third column details the response code and result.


Let’s start building your first environment!

**Step 1)** Create a new GET request from https://reqres.in/api/users?page=2 for a user list.


**Step 2)** Submit both GET requests to ensure you are receiving a status 200.
 
**Step 3)** Under Params, enter a key and value pair. The key being page and value is 2. The key is a variable placement holder and the value gives it a replacement value.

**Step 4)** Create a new environment by clicking on the ‘+’ tab or by the wrench icon next to the eye icon on the top right corner. In this example, the wrench was used. A new window will pop called ‘Manage Environments’. 

**Step 5)** Click add to go on to the next screen and the blank form should appear.

> Note: Click on the breadcrumbs to delete or remove the environment list.

**Step 6)** Name this environment ‘Stage’ and complete the row as ‘page’ for variable and ‘2’ for the initial and current value.

**Step 7)** Change the 2 of the url to a new endpoint called {{page}}. Notice how the previous key value has now changed to page and {{page}}. If you hover over the endpoint variable, an error will appear.

> Note: An error was caused because in this environment there is no numbered value given for this variable, therefore the request is not valid. The page requires a variable.

**Step 8)** Change the environment to the previously created ‘Stage’ completed in Step 6. 

**Step 9)** Hover of the endpoint again and now it should be green and present the a number value. 

> Note: The error has now resolved as a variable has been set.

> Note: If you click on the eye icon,  you can see the same details.

**Step 10)** Create a copy of the Stage environment put going to wrench icon again. Click on the breadcrumb icon and to create the copy. 

**Step 11)** Click on the Stage Copy in order to modify the environment.

**Step 12)** Rename the environment to ‘Production’ and change the initial and current value to 3. 

**Step 13)** Click update.

**Step 14)** Click on Globals at the bottom of the screen. Here we will make a new variable endpoint that will be accessible globally (available in any environment).

**Step 15)** Set the variable to URL and the initial and current value to “https://reqres.in”. 

**Step 16)** Change the url to the new endpoint called {{URL}}.

**Step 17)** Change the environment to Production and click send. You should see the body change below.

Congratulations, you have now created not only one environment, but two!
Environments can be useful when you need to use different variables in different environments to change. 
