---
layout: default
title: Working With Environments and Variables
nav_order: 4
---

# Working with Environments and Variables
---

### Understanding Variables
 A variable can be used as a reference tool and be defined with a specific value that a user sets. This tool can be useful when the variable exists in different places and may be changed at one place. Thus user requests are more efficient and readable. 

### Understanding Environments 
An environment allows for collections and requests to be run against different data sets. You can have different environments meant for testing, development, and production that will need different data sets to be passed. In this application, environments are made up of key-value pairs of variables, and each variable represents its key. You may access it by referencing the variable. Let’s get started by creating your first environment.
For the example below, we will be taking sampel data from this website: reqres.in. On the site, there are a list of fake GET, POST, PUT, DELETE requests that can be made. The second column shows how to mock your request, and the third column details the response code and result.

Let’s start building your first environment!

**Step 1)** Click on the ‘+’ button in the top left corner. A pop-up screen will appear and you can click on ‘Environment’ to add a new environment to Postman.

**Step 2)** Add a new environment by giving a new name. We have called this new environment “QA”.
 
**Step 3)** Click add to go on to the next screen and the new environment should appear.
Note* Click on the breadcrumbs to delete or remove the environment list.

**Step 4)** Click the blue ‘save’ to save the GET repost to the newly created environment and a new window will appear. Click ‘X’ on to close the window.

**Step 5)** Create a new request and save it under the POST collection. If you are not sure what collections are, please refer to the previous section on collections. For this example, we have saved this request as “User Registration”.

> Note: On the left side panel, you can see how the collections are being saved and which environment or collection each request belongs to.

**Step 6)** Add the link provided at the start of the section and change the request to POST.

**Step 7)** Change to the body tab located beneath the url. Add in the object (insert code snippet) which includes two key-value pairs: email and password.

**Step 8)** Click the blue ‘Send’ button. Now it returns an error response of ‘400 Bad Response’. Luckily, the error message is able to give us a hint to what is causing the error.

> Note: Error was caused due to the formatting of the text. When the post response is sent, it cannot read the content in plain text.

**Step 9)** Go to the ‘Headers’ tab located next to body, and add a new key-value pair of ‘Content-Type’ and ‘application/json’, respectively. 

**Step 10)** Click send again and the status code should be 200.

**Step 11)** Go back to manage environments and enter the following the following and click update:

(insert markdown table)

variables: endpoint, username, and password
Initial Value: /api/register, sidney@fife, pistol

**Step 12)** Replace all initial values to their respective variables by adding {{variable}}.
