---
layout: default
title: Creating Postman Collections
nav_order: 4
---

# Creating Postman Collections
---
Collections in Postman are a compiled series of requests within a specific environment. This tool is most useful for API testing and the requests are done one after another.

<br>

When you click on the Runner button, it should load up a new screen which looks like this:

## How To Create A Postman Collection
Collections are a group of requests saved in one folder. The requests can be GET, POST, PUT, or DELETE.

> Note: We will be using reqres.in as the sample REST API. There are many types of fake requests you may use to run the sample collection.

**Step 1)** Create a new collection folder called ‘Testing’ by clicking the top left orange ‘+’ button and save.

**Step 2)** Create a new request called ‘GET userList’ and save it in your collections named ‘Testing’.

**Step 3)** Add the request from reqres.in to the end of the url and click send. You should see a code 200 OK.
 
 
**Step 4)** Repeat step 2 and 3, but create a new GET request called “GET singleUser” and add [https://reqres.in/api/unknown/1](https://reqres.in/api/unknown/1) to the URL. 

**Step 5)** Click on the breadcrumbs on the left-side panel in the Testing tab and select view more actions to add a new sub-folder called ‘GET’. Place the two previously created GET requests into that new folder.

**Step 6)** Click on the arrow button above the bread crumbs and a new sub-window will appear to the right.

**Step 7)** Click the blue ‘Run’ button and a new window appears called “Collection Runner”. Here you can run the test as many times as you want. We will run this collection twice. To do this, you will have to change the iterations to two. Finally click ‘Run Testing’.

**Congratulations**, you just ran your first collection! Your run results should be generated on a new window and look like the below.


Run Summary Report
