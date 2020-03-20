---
layout: default
title: Working With Requests
nav_order: 3
---

# Working With Requests
---

POST requests work differently than GET requests from the user adding data to the endpoints through data manipulation. We will be handling POST requests in this section of the guide. Using the same data set from the previous section, we will begin with adding a new user.
<br>

**Step 1)** Click a new tab to create a new request.

![New Request](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-1.png)

**Step 2)** In this new tab:
1. Set your HTTP request to POST.
2. Input the link in request url: [https://jsonplaceholder.typicode.com/users](https://jsonplaceholder.typicode.com/users)
3. Switch to the Body tab.

![POST Request](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-2.png)

**Step 3)** In the Body:
1. Click raw.
2. Select JSON.

![RAW JSON](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-3.png)

**Step 4)** Copy and paste:

1. A user result from the previous GET request. Make sure the code is copied correctly, you will notice paired curly braces and brackets.
2. Change the ID to 11 and to “Your Name”.

<br>

**Code snippet:**

```{
   "id": 11,
    "name": "Jane Smith",
    "username": "Bret",
    "email": "Sincere@april.biz",
    "address": {
      "street": "Kulas Light",
      "suite": "Apt. 556",
      "city": "Gwenborough",
      "zipcode": "92998-3874",
      "geo": {
        "lat": "-37.3159",
        "lng": "81.1496"
      }
    },
    "phone": "1-770-736-8031 x56442",
    "website": "hildegard.org",
    "company": {
      "name": "Romaguera-Crona",
      "catchPhrase": "Multi-layered client-server neural-net",
      "bs": "harness real-time e-markets"
    }
  }
```
<br>
 
**Step 5)** Next:
1. Click Send.
2. “Status: 201 Created” should now be displayed
3. Data should now show up in the body.

![Body](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-4.png)

> Note: Post request should have the correct format to ensure that requested data will be created.

<br>

**How to Parameterize Requests**

One of the most useful features in Postman is Data Parameterization. This feature helps avoid repetition of the same tests and iterations can be used for automated testing. Rather than creating the same requests with different data, you can set variables with parameters. This data can be an environment variable or data file. In the next section, we will discuss how to work with environment variables.
<br>

Parameters are created through the use of double curly brackets: {{sample}}. Let's create a parameterized POST request.

**Step 1)** Set your HTTP request to POST.
1. Input this link: [https://jsonplaceholder.typicode.com/users](https://jsonplaceholder.typicode.com/users). Replace the first part of the link with a parameter such as {{url}}. Request url should now be {{url}}/users.
2. Click send. (There should be no response because we have not set any parameters)

![No Response](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-5.png)

**Step 2)** To use the parameter you need to set the environment

1. Click the eye icon.
2. Click edit to set the variable to a global environment.

![Global](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-6.png)

**Step 3)** In variable,

1. SET name to the url which is [https://jsonplaceholder.typicode.com](https://jsonplaceholder.typicode.com_)
2. Click Save.

![Save](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-7.png)

**Step 4)** Click close if you see the next screen.

**Step 5)** Go back to your POST request then click send. The results from your request should now populate.

> Note: To avoid errors, remember to set your parameters to that they have a source like an environment variable or data file.

![Errors](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/working-requets-8.png)

**Congratulations**, you just created a POST request in Postman! In addition to the previous [section](https://cee-elle.github.io/postman-documentation/docs/composing_requests/), you should now have a good understanding of creating GET and POST reqeusts using Postman! Give a hand to yourself.
