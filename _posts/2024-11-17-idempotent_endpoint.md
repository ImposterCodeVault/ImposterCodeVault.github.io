---
title: Idempotent Endpoint
date: 2024-11-17 13:35:00 +1300
categories: [tutorial]
tags: [webapi, idempotent]
---

# Creating an Idempotent Post endpoint in a Dotnet Web API

* TODO: Give some background on idempotency in Rest APIs, and which methods are idempotent already, and which will need to handle this in some way.

The Http standard for post requests is that they are idempotent
* This means that no matter how many times you send the request, the result on the server will be the same. You may get a different response back, but the state of the server remains the same.

In this blog post we'll look at how to make a POST endpoint idempotent to ensure the validity of the data on the server side.

As a beginning, we'll create a dotnet web api by opening up the Visual Studio Code within a directory, and running the following command:

``` bash
dotnet new webapi 
```

This will create us a new Dotnet Web API project (using minimal api over controllers), where we can create a small proof of concept around making a post endpoint idempotent.

* Note that the name of the project will be the same as the folder in which you created it. In my case the folder was named "IdempotentAPI". If you want to give the project a different name, you can add a flag to the command like so:
  * ``` bash
    dotnet new webapi -o MyProjectName
    ```
Your program.cs should look like this:




TODO: Finish copying this post over from blogger once website is deployed
