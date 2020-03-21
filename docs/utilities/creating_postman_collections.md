---
layout: default
title: Creating Postman Collections
nav_order: 5
---

# Creating Postman Collections
---
Collections in Postman are a compiled series of requests within a specific environment. This tool is most useful for API testing. It is also a group of requests saved in one folder and made to execute one after another. The requests can be GET, POST, PUT, or DELETE.

> Note: We will be using https://reqres.in as the sample REST API. There are many types of fake requests you may use to run the sample collection.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-3.png)

**Step 1)** Create a new collection folder called ‘Testing’ by clicking the top left orange ‘+’ button and save.

![Testing](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-4.png)

**Step 2)** Create a new request called ‘GET userList.

![GET](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-5.png)

1. Save it in your collections named ‘Testing’

![Testing](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-6.png)

**Step 3)** Add the request from reqres.in to the end of the url and click send. You should see a code 200 OK.
 
 
**Step 4)** Repeat step 2 and 3, but create a new GET request called “GET singleUser” and add [https://reqres.in/api/unknown/1](https://reqres.in/api/unknown/1) to the URL. 

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-7.png)

**Step 5)** Click on the breadcrumbs on the left-side panel in the **Testing** tab.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-8a.png)

1. Select view more actions to add a new sub-folder called ‘GET’.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-8b.png)

2. Place the two previously created GET requests into that new folder.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-8c.png)


**Step 6)** Click on the arrow button above the bread crumbs and a new sub-window will appear to the right.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-9.png)

**Step 7)** Click the blue ‘Run’ button and a new window appears called “Collection Runner”. Here you can run the test as many times as you want. We will run this collection twice. To do this, you will have to change the iterations to two. 

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-2.png)


**Step 8)** Click ‘Run Testing’.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-10.png)




**Congratulations**, you just ran your first collection! Your run results should be generated on a new window and look like the below.

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-11.png)

Run Summary Report

![Runner](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/postman-collections-12.png)

Now that you have built your first collection, you will be able to test mulitiple requests. You can also create different sets of collections to test within the same or different environment. 
