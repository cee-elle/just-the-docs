---
layout: default
title: Composing Requests
nav_order: 2
---


# Composing Requests
One of Postman's primary purposes is allowing us to craft requests to the APIs we use. This section will guide you to making your first request with Postman! In order to make a request of the API, start by:

    Note: We will be using content from https://jsonplaceholder.typicode.com/users to simulate a JSON file.

**Step 1)** In Postman, click a new tab to create a new request. 

**Step 2)** In the new tab:
1. Set your HTTP request to GET.
2. Input the link in request url: https://jsonplaceholder.typicode.com/users

**Step 3)** Next,
Click Send.

*Alternatively, you can click the dropdown arrow attached to the send button, and choose send and download. This will provide you with a save file of the response.*

Status: 200 Created should be displayed

*You'll see a message that echoes some header values along with a message, which reads the API is listening.*

Posted data are showing up in the body.

*If you receive an error instead of the expected text, verify that the sample API is running, that you've entered the correct URL, and the get method is selected.*

<br>

### The response body is presented under the body tab with three views:
**Pretty** - Applies basic formatting to content and is the default setting.

**Raw** - Displays content exactly as it was received.

**Preview** - Attempts to render content. Useful when you are trying to get an idea of how an HTML document appears in the browser.

    Note: When the response is an image or other non-text type, these options won't be available. 

<br>
**Congratulations**, you have made your first API request in Postman! 
