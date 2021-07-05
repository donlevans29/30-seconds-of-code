---
title: Return Promise into JSON
tags: api,json
firstSeen: 2021-07-04 T05:00:00-04:00
---

Returns Promise into JSON format

- Takes your api url and any other parameters for the requested url and returns back a promise then turns the
promise response into json formate.
- You simply input your api key and api url with params
- Now data should be ready for your retrieval functions

```js
let API_KEY = "yourUniqueApiKey";

const getData = arguments => {
   const URL = "https://yourapiurl.org";
   const FULL_URL = `${URL}?q=${param}&appid=${API_KEY}&`;
   const namePromise = fetch(FULL_URL)
    return namePromise.then((Response) => {
      return Response.json()
    })

  }
```
