# Prepare your Node.js application for production in Kubernetes

We've recently published an npm library for Node.js applications that provides useful common functionalities, like graceful error handling & shutdown, structured JSON logging and several HTTP middleware to make your application truly ready production environments.
In this blog post I will

## Graceful error handling

In Node.js you can register error handlers for uncaught exceptions and unhandled Promise rejections. We are all humans and errors can slip into our code, edge cases we haven't prepared it for. What happens when an unexpected error is thrown which we are not catching? Our program exits right away, possibly leaking resources, loosing session data and leaving in-progress requests unfinished. We really want to avoid this to happen!

Consider the following example:

```js
const
```
