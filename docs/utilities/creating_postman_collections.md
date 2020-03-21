---
layout: default
title: Creating Postman Collections
nav_order: 5
---

# Creating Postman Collections
---
Collections in Postman are a compiled series of requests within a specific environment. This tool is most useful for API testing. It is also a group of requests saved in one folder and made to execute one after another. The requests can be GET, POST, PUT, or DELETE.

> <mark>Note:</mark> We will be using https://reqres.in as the sample REST API. There are many types of fake requests you may use to run the sample collection. 

**Step 1)** Create a new collection folder called ‘Testing’ by clicking the top left orange ‘+’ button and save.

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-1.png)

**Step 2)** Create a new request called ‘GET userList.

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-2.png)

1. Save it in your collections named ‘Testing’

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-3.png)

**Step 3)** Add the request from reqres.in to the end of the url and click send. You should see a code 200 OK.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-4.png)
 
**Step 4)** Repeat step 2 and 3, but create a new GET request called “GET singleUser” and add [https://reqres.in/api/unknown/1](https://reqres.in/api/unknown/1) to the URL. 

**Step 5)** Click on the breadcrumbs on the left-side panel in the **Testing** tab to add a folder.

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-5.png)

1. Name the new sub-folder called ‘GET’.

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-6.png)

2. Place the two previously created GET requests into that new folder.

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-7.png)


**Step 6)** Click on the arrow button above the bread crumbs and a new sub-window will appear to the right.

![](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-8.png)

**Step 7)** Click the blue ‘Run’ button and a new window appears called “Collection Runner”. Here you can run the test as many times as you want. We will run this collection twice. To do this, you will have to change the iterations to 2. 


**Step 8)** Click ‘Run Testing’.

**Congratulations**, you just ran your first collection! Your run results should be generated on a new window and look like the below.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-10.png)

<mark>Note:</mark> This what a Run Summary Report looks like if you like to review all the tests and the results of each iterations.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/collections-11.png)

Now that you have built your first collection, you will be able to test multiple requests. You can also create different sets of collections to test within the same or different environment. There is a summary report that will show the number of iterations, as well as what has passed and failed.
