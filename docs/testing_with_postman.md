---
layout: default
title: Testing With Postman
nav_order: 7
---

# Testing With Postman
---

Postman Tests are a set of JavaScript codes embedded into the requests that help you verify results of your tests successful or failed status. You can compare results with your previous testing and usually start with a pm.test. 

Let's create some basic tests for our parameterized requests from the “Working with Requests” section.

**Step 1)** Go to your GET user request.
1. Switch to the tests tab (located on the right side “snippet codes”).
2. From the snippets section, click "Status code: Code is 200" (The pane is auto-populated).

**Step 2)** Click Send. The test result should now be displayed.

![Send Test](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/testing1.png)

**Step 3)** Go back to the test tab and let's add another test. 
1. This time we will compare the expected result to the actual result. 

> Reminder to change your request to GET and your previously entered information from Step 4 in “Working with Requests” still exists in the Body tab.

2. From the snippets section, click on "Response body:JSON value check".

**Step 4)** Checking your results.
1. Replace "Your Test Name" from the code with "Check if the user with id1 is Your Name".
2. Replace jsonData.value with jsonData[0].name.

*To get the path, check the body in POST result from earlier. If you want to get the second result, use jsonData[1] and so on for incremental results.*

3. Locate in “to.eql(“_________”);”, input “Your Name”.

**Step 5)** Click send. There should now be two passed test results for your request.

> Note: Different kinds of tests can be created in Postman. Explore the tool and see which tests fit your needs.

![Send Test](https://raw.githubusercontent.com/cee-elle/postman-documentation/gh-pages/docs/raw/testing2.png)

**Great job!** You have come along way from understanding and creating your first request to now testing them in Postman! How does it feel? 
