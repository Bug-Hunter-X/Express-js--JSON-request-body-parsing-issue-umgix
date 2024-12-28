# Express.js JSON Parsing Bug

This repository demonstrates a common issue encountered when working with JSON request bodies in Express.js applications.  The problem arises when the `Content-Type` header in the request is missing or incorrectly set, preventing Express from correctly parsing the JSON data.

## Bug Description

The `bug.js` file contains an Express.js app that attempts to handle POST requests with JSON data. However, if the request does not include a `Content-Type: application/json` header, the `req.body` will be empty, leading to unexpected behavior and potential errors. 

## Solution

The `bugSolution.js` file provides a solution to this issue by implementing middleware to check the request content type and parse accordingly. 
