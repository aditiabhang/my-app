# Cloudflare Project

Deployed a Cloudflare Workers project that builds a linktree-style website.

### Deployed a JSON API
As a first step, I created a new Workers project using Wrangler. It responds to two kinds of requests, one to generate a JSON API, and second, to serve an HTML page 

To begin, I defined an array of links in Javascript with number of link objects, each with a name and URL string. Like below example for one of these link objects:

```json
{ "name": "Portfolio", "url": "http://aditiabhang.github.io/" }
```

I have defined a few links in this array. (Go visit my final project and check em out..!!

Once I defined this array, I set up a request handler to respond to the path `/links`, which returns the array itself as the root of the JSON response.

In addition, I also ensured that the API response has the correct `Content-Type` header to indicate to clients that it is a JSON response.

> Screenshots:

### LinkTree Style Website

<img width="1440" alt="Screen Shot 2020-10-28 at 3 55 58 PM" src="https://user-images.githubusercontent.com/51350594/97496463-f8ead500-1936-11eb-9b39-86e62a66145f.png">


### Request Handler JSON Response

<img width="1072" alt="Screen Shot 2020-10-28 at 3 56 25 PM" src="https://user-images.githubusercontent.com/51350594/97496469-fab49880-1936-11eb-84bc-e9adb97afad6.png">