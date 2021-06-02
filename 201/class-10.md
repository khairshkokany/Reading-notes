# JS 
## Effective Debugging and Error Handling for JavaScript

**Over the past few decades, JavaScript has evolved from a simple browser-based scripting to an advanced programing language, becoming an integral part of modern web applications. The advancement of web browsers, standardization, browser and third-party debugging and error handling solutions, enables both JavaScript development and error investigations in production more productive.**

**Debugging is a process for testing, finding the errors and reducing them from happening in future. Debugging JavaScript either requires having support for JavaScript debugger keyword, breakpoint support with web browser tools, or third-party tools. These tools range from browser plugins like Augury which is an Angular development and debugging extension for Chrome, third-party tools & more. It is also possible to use 'debugger' keyword support (depending on the browser type and version) and to freeze the code at a given point and investigate the issue. Let us look at few popular debugging and error handling tools.**


## Effective Debugging

### Chrome Browser Tools


<img src="https://lh5.googleusercontent.com/UwljoUkDvmwhnAC42-YN7zvU2JQcK6ceTOrtjWxGFV7R4unAWnEwKBPkyG8s7WAjpDsHZuZ4Bcv1SPWtR7EscRiMlY4NgTn5h5vOWssq2VG0wzpXHBHu6hbGNedwZqiZL-d7cWsv">

> This is my favorite tool for JavaScript development. One of the features I often used is to map the local file system to the loaded file in JavaScript development environment so that it is possible to debug the file using breakpoints of debugger keyword while saving the changes to the files directly in Sources section in the browser. In addition, it is possible to use the console.log command to log any variables or text to the Chrome browser console to investigate any issues.

<img src="https://lh6.googleusercontent.com/6IuYE7hqFkCb45_Vidh6Dcq8ls3ZM7tDgNxQzEldsLMaM1TJvT8I4gnFImdWZj9ylyLS68GXWE-F3lktiKI-FbvOIdMXiS5nzF9lAfAChr-JHZHMMEbyUnIIWbr4KrVcSYzmwGuo">


### Third-Party Services

**There is a large number of emerging third-party services, that support JavaScript debugging and error handling, such as Bugsnag’s error monitoring platform. These tools provide insights of what's going on with the code running in various user's browsers so that it is possible to notify the development team with details of the issues with errors being logged. The main advantage of these types of services is that they provide the debugging and error handling remotely as a service so that it is possible to capture this valuable information to easily investigate an issue.**

### Online and Desktop IDEs


**Using Integrated Development Environments (IDEs) is the most popular ways to debug JavaScript Applications today. With the tight integration with browser tools, it is now possible to debug the code either from Online or Desktop IDEs, where it is possible to use the features like error logging, using keywords to break the code and using breakpoints. The advantage of this approach over the rest of the tools is that it is possible to investigate the issue from all the angles including the backend code.**

## Effective Error Handling and Logs

### Handling Log Levels

**When developing JavaScript applications it is important to have different levels of logging enabled. For example, when the application runs in testing or staging environments, it is possible to enable detailed logging including application flow, important variables & etc. while in production environments only to log errors. To achieve these, either a third-party JavaScript library or a custom implementation is required to manage log-levels.**

### Log Transport

**Since JavaScripts runs on client's browser, an error occurred remotely needs to be transferred to a new environment so that the development or ops team can investigate by accessing the logs.**

### Log Formats

**It is also important to have a format which is possible to be extended in future to support any new log data formats as well as to keep uniformity across different logging messages.**

### Exception Handling

**This is one of the key areas, where it is required to effectively handle the errors and show users with sufficient information about the situation and pass that information to the developer. This can also be handled based on Log Levels.**