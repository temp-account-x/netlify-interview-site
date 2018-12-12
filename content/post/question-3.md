---
title: "Question 3"
date: 2018-12-11T21:46:18-08:00
draft: true
---
## What did you think of our service during the time you used it?  Provide either some constructive criticism or some points that impressed you.  Be honest!  “It sucked” isn’t a wrong answer unless you don’t elaborate and provide some constructive criticism ;)

First, I was surprised by the 'it just works' aspect of Netlify. I was concerned about what would happen if I ran into problems with the deploy. Nope. I clicked the 'Deploy site' button and the next thing I knew, my little static site was being served by the Netlify CDN.

For example, I was expecting Netlify to just vacuum up the ./public directory used by Hugo for the static site content, but my github repo contained the source files Hugo uses to build the static site. Would I have to configure something special to get Netlify to deploy the public directory? Nope again! Netlify actually runs the Hugo site build command and builds the site itself.

As far as criticism, I just want to know how it works - like I might for a magic trick on stage. Yes, it is a great magic trick. Now, may I please go backstage with you, the magician, and have you show me exactly how the trick works? Please?
