---
title: "Question 4"
date: 2018-12-11T21:46:15-08:00
draft: false
---

## Talk about how you made your site and why you chose the tools you did.  Briefly explain a challenge you experienced in setting up this site and how you solved it.

Interestingly, I first used the Hugo site I set up in 2017 which hasn't seen much use recently. I used Hugo back in 2017 because I liked the simplicity of it's syntax (TOML) and it seemed to be a relatively active project. I really liked a specific theme (the Nix theme by LordMathis) and this was a large factor in my decision to use Hugo. That it is written in Go is another big selling point.

However, this was me missing that the site I create should contain these answers to the test! I therefore needed to make a new Hugo site (not use my existing one).

For the new site, I chose the KISS theme because I believe in the [KISS principle](https://en.wikipedia.org/wiki/KISS_principle). I was also just trying to 'get it done' not make it look fancy.

My original Hugo site was deployed from a personal system (the web server is in my home). When I update the site locally I use a bash script to automate pushing the updated content the site root used by Nginx. Then getting SSL working and configured was another learning process (Let's Encrypt).

I think you have just made a customer as I am sold! With Netlify, now all I need to do is push my updated site to Github and Netlify will both rebuild the site and also handle the Let's Encrypt certificates.

I didn't realize Netlify already would do these things for me. Why wasn't I using Netlify before this application process?!?!

Last but not least, one of my biggest challenges was how to include a theme in my git repo which itself was a git repo. I didn't know much about the git submodule command. I used it based on a recommendation from git itself only to later find out (in the [Hugo docs](https://gohugo.io/getting-started/quick-start/#step-3-add-a-theme)) that I had done so correctly. However, this caused the site not to build as I made modifications to the theme and I couldn't push those to the master repo (nor should I). Then I got to learn about how hard it is to remove submodules in git so I could add the theme again, this time not as a submodule. This was a learning experience to say the least.
