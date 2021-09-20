# Status Codes Based On REST Methods

## In your own words, describe what each group of status code represents:

 100’s =  informational status codes

 200’s =  success codes

 300’s =  redirection codes

 400’s =  client error codes

 500’s =  server error codes

## What is a status code 202?

Created -  This code should signal backend-side resource creation and come along with a Location header that defines the most specific URL for that newly created resource

## What is a status code 308?

Permanent Redirect -This tells the client to use another URL to access the resource and not use the current URL anymore

## What code would you use if an update didn’t return data to a client?

406 Not Acceptable

## What code would you use if a resource used to exist but no longer does?

410 Gone

## What is the ‘Forbidden’ status code?

403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

# Build A REST API With Node.js, Express, & MongoDB - Quick 

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?

becase when we will deploy this application we will not use the local host 

## What is middleware?

code that runs when the server gets the request but before it passed to ypur routs

## What does app.use(express.json()) do?

lets our server accept json as a body instead of post element 

## What does the /:id mean in a route?

 used for getting one and the id means that this have a parameters (we can access parameters using `req.param.id` or whatever the params name)

## What is the difference beween PUT and PATCH?

PUT --> update all the information all at once

PATCH --> update based in the user passes 

## How do you make a defalut value in a schema?

by setting a defualt prameter 

## What does a 500 error status code mean?

500 -- that tere are error in your server


resorses 

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

[Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)