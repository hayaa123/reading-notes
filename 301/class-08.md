# API Design Best Practices

## What does REST stand for?

Representational State Transfer

## REST APIs are designed around a resources.

## What is an identifer of a resource? Give an example.

 URI that uniquely identifies that resource

 ```
https://adventure-works.com/orders/1
 ```

## What are the most common HTTP verbs?

GET, POST, PUT, PATCH, and DELETE.

## What should the URIs be based on?

based on nouns (the resource) and not verbs (the operations on the resource).

## Give an example of a good URI.

```
https://adventure-works.com/orders // Good
```

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

expose a large number of small resources ,bad thing

## What status code does a successful GET request return?

200

## What status code does an unsuccessful GET request return?

404

## What status code does a successful POST request return?

201

## What status code does a successful DELETE request return?

400

## Things I want to know more about

more applicattion af these requests

### resorses 

[this plog](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)