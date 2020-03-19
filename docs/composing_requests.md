---
layout: default
title: Composing Requests
nav_order: 2
---


# Composing Requests
---
One of Postman's primary purposes is allowing us to craft requests to the APIs we use. This section will guide you to making your first request with Postman! In order to make a request of the API, start by:

> Note: We will be using content from [https://jsonplaceholder.typicode.com/users](https://jsonplaceholder.typicode.com/users) to simulate a JSON file.

<br>

**Step 1)** In Postman, click a new tab to create a new request. 

![New Request](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-1.png?raw=true)

**Step 2)** In the new tab:
1. Set your HTTP request to GET.
2. Input the link in request url: https://jsonplaceholder.typicode.com/users

![GET Request](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-2.png?raw=true)

**Step 3)** Next,
1. Click Send.

![Sending Request](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-3.png?raw=true)

*Alternatively, you can click the dropdown arrow attached to the send button, and choose send and download. This will provide you with a save file of the response.*

![Send](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-4.png?raw=true)

2. Status: 200 Created should be displayed

*You'll see a message that echoes some header values along with a message, which reads the API is listening.*

![Posted Data](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-5.png?raw=true)

3. Posted data are showing up in the body.

*If you receive an error instead of the expected text, verify that the sample API is running, that you've entered the correct URL, and the get method is selected.*

![Response Body](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-6.png?raw=true)

### The response body is presented under the body tab with three views:
**Pretty** - Applies basic formatting to content and is the default setting.

**Raw** - Displays content exactly as it was received.

![Raw Body](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-7.png?raw=true)

**Preview** - Attempts to render content. Useful when you are trying to get an idea of how an HTML document appears in the browser.

> Note: When the response is an image or other non-text type, these options won't be available. 

![Preview Body](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/Creating_Requests-9.png?raw=true)

**Congratulations**, you have made your first API request in Postman! 
