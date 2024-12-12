# ROUTING(--routing)

When you run the command ng new angular-app --routing, the --routing flag tells Angular to set up routing functionality for your newly created Angular application.

## What does this mean?
In Angular, routing refers to the ability to navigate between different views (or components) within the application. It allows you to change the view based on the URL in the browser, without having to reload the entire page. This is essential for building single-page applications (SPAs) where different  content is displayed based on user interactions, all without a full page reload.

## What happens when you use --routing?
1. Routing Module: Angular will automatically generate a file called app-routing.module.ts in the src/app directory. This module is used to configure the routes in your application. Inside this file, you will define paths and map them to specific components.
2. Update App Module: The newly generated application will also automatically import and include AppRoutingModule in the main AppModule (app.module.ts).
3. Routing Setup: The routing module provides the necessary imports and configuration to set up routing in the application. You can later modify this module to define your routes and specify how the navigation between components will happen

# GUARD

Guards are a powerful feature in Angular for controlling navigation and protecting routes based on specific conditions. By using guards, you can secure routes, prevent users from leaving pages with unsaved data, load data before navigation, and prevent unauthorized access to certain parts of your app. Understanding and effectively implementing guards is a key part of building robust, user-friendly Angular applications.

## Types of grard
1. CanActivate
2. CanActivateChild
3. CanDeactivate
4. Resolve
5. CanLoad

# RxJS & Observable 

## Observable
Think of an Observable like a stream of data. It's like a pipe where data flows through, and you can "watch" it as it moves. An Observable lets you:
1. Listen to the data as it changes.
2. React whenever new data arrives.
3. Handle the data in a way that is clean and organized.
   
Imagine you're watching a weather station. The Observable is the station, and the data it provides is like weather updates — each update could be rain, snow, sunshine, etc. You can "subscribe" to the weather station, and whenever there’s a new update, you’ll get it instantly.

## RxJS
RxJS stands for Reactive Extensions for JavaScript, and it's a library that makes working with Observables easier. It provides tools to manage, transform, and combine streams of data. So, with RxJS, you can:

1. Create Observables from different data sources (like events, timers, HTTP requests).
2. Combine or filter the data in real-time.
3. Handle complex scenarios where you need to deal with multiple streams of data.

A Simple Example
Let’s say you have a button, and each time you click it, you want to log something. Without RxJS, you'd write event listeners in plain JavaScript. But with RxJS:
1. The button click can be treated as an Observable (like a stream of button presses).
2. You can subscribe to it, and whenever the button is clicked, the click event is passed on and handled in your code.
In simple words, Observable is a tool to manage data that arrives over time (like button clicks, data fetching, etc.), and RxJS is a powerful library that makes it easy to work with those streams of data in a clean and efficient way.




