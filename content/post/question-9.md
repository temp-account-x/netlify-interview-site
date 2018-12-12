---
title: "Question 9"
date: 2018-12-11T21:46:05-08:00
draft: false
---

## Can you set up a redirect from “/netlify/anything” to https://www.google.com/search?q=anything ?

I thought adding the following to `static/_redirects` would do the trick:

```
/netlify/* https://www.google.com/search?q=:splat 200
```

This does redirect to google but does not include the text after /netlify/ in the URL to be included in the search. I would love to know what I am missing as it seems I am close, but not exactly correct.

Here is an example URL:

https://netlify.of-mu.org/netlify/example
