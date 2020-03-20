---
layout: default
title: Troubleshooting
nav_order: 8
---

# Troubleshooting
---


### Unable to Load

If you see the window appear when trying to load up the application, please delete your postman application and its local files and reinstall the latest version. 

![](https://github.com/cee-elle/postman-documentation/blob/gh-pages/docs/raw/troubleshoot-1.png)

> Note: By deleting your local files, all local saved files will be permanently deleted. If you have a Postman account, ensure your account is actively synced when logging into the web application.

```
“Could not get any response” Error
You may get an error that looks like this:
Could not get any response.
There was an error connecting to localhost:3001/blocks.
Why this might have happened:
The server couldn't send a response:
Ensure that the backend is working properly
Self-signed SSL certificates are being blocked:
Fix this by turning off 'SSL certificate verification' in Settings > General
Proxy configured incorrectly
Ensure that proxy is configured correctly in Settings > Proxy
Request timeout: Change request timeout in Settings > General
```

In order to fix this, you will have to go to your settings tab and turn off the “SSL certificate verification” tab.

### Archived Files
If you would like access to your archived files, you may go to “https://go.postman.co/usage/archive” where you will receive a JSON file. Another option is to export it from your application. 

#### How to export and import your archived files:
   **Step 1)** Create a new Workspace to import the restored Collections
   **Step 2)** Go to Settings tab or click on the wrench at the top right corner and under Data, click to download the file.
   **Step 3)** Go to Settings again and this time choose the file to open this time.

### Incorrect URLs or Undefined Variables

Ensure that your variables in either or both your global or environmental settings are defined with values. Request variable errors may return a 404 Bad Request  or incorrect server address.

### Incorrect protocol

If you are running to protocol errors, recheck if your urls are starting with "https://" instead of "http://" or the other way around.
