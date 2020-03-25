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

For the example below, you will be taking samplee data from this website: https://reqres.in. On the site, there are a list of fake GET, POST, PUT, DELETE requests that can be made. The second column shows how to mock your request, and the third column details the response code and result.


Let’s start building your first environment!

**Step 1)** Create a new GET request from https://reqres.in/api/users?page=2 for a user list.

**Step 2)** Submit both GET requests to ensure you are receiving a status 200.
 
**Step 3)** Under Params, enter a key and value pair. The key is page and value is 2. 

> <mark>Note:</mark> The key is a variable placement holder and the value gives it a defined value.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-A.png)

**Step 4)** Create a new environment by clicking on the ‘+’ tab or by the wrench icon next to the eye icon on the top right corner. In this example, the wrench was used. A new window will pop called ‘Manage Environments’. 

**Step 5)** Click add to go on to the next screen and the blank form should appear.

> <mark>Note:</mark> Click on the breadcrumbs to delete or remove the environment list.

**Step 6)** Name this environment ‘Stage’ and complete the row as ‘page’ for variable and ‘2’ for the initial and current value.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-B.png)

**Step 7)** Change the 2 of the url to a new endpoint called <font color="maroon">{page}</font>. Notice how the previous key value has now changed to page and <font color="maroon">{page}</font>. If you hover over the endpoint variable, an error will appear.

> <mark>Note:</mark> An error was caused because in this environment there is no numbered value given for this variable, therefore the request is not valid. The page requires a variable.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-C.png)

**Step 8)** Change the environment to the previously created ‘Stage’ completed in Step 6. 

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-D.png)

**Step 9)** Hover of the endpoint again and now it should be green and present the a number value. 

> <mark>Note:</mark> The error has now resolved as a variable has been set.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-E.png)

> <mark>Note:</mark> If you click on the eye icon, you can see the same details.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-F.png)

**Step 10)** Create a copy of the Stage environment put going to wrench icon again. Click on the breadcrumb icon and to create the copy. 

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-G.png)

**Step 11)** Click on the Stage Copy in order to modify the environment.

**Step 12)** Rename the environment to ‘Production’ and change the initial and current value to 3. 

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-H.png)

**Step 13)** Click update.

**Step 14)** Click on Globals at the bottom of the screen. Here we will make a new variable endpoint that will be accessible globally (available in any environment).

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-I.png)

**Step 15)** Set the variable to URL and the initial and current value to “https://reqres.in”.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-J.png)

**Step 16)** Change the url to the new endpoint called {{URL}}.

**Step 17)** Change the environment to Production and click send. You should see the body change below.

![KeyValue](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/enviro-K.png)

**Congratulations**, you have now created not only one environment, but two!

Now that you have created some environments, you can run same collections in different environments to verify your reslts. Each environment should have different values in order to properly test your requests. You should now have some understandings of how global and environment variables work in Postman.
