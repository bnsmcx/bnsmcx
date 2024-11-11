# Hi there, I'm Ben Simcox 👋

I'm a software engineer writing mostly backend Go though I (not so) secretly love TUIs and do my best to find an excuse to shoe horn one in to every project.

The following is an overview of all of the public work I have hosted here on Github.  Much of it was short lived experimentation or tinkering while some stuff has more depth.  Hopefully all of it helps you get a sense of who I am as a developer.

## yVPN

I've worked on a series of VPN management tools all of which I've named yVPN. My great grandmother had a series of pugs named Tigger, perhaps that was the subconcious motivator.  yVPN is short for "your VPN" which is a little confusing since nobody else uses it.  "My VPN" didn't sound as cool I guess.

This series of projects arose to make it more convenient for me to spin up my own VPN servers on Digital Ocean.  I'd been doing this by hand for years because it was cheaper to just pay for a Droplet and it was simple enough to get OpenVPN up and running by hand in somewhat less than an hour.  It was easy enough but I saw that this was an option available to me because I had the skill set to set it all up myself whereas my non-technical friends and family were at the mercy of whatever commercial solutions were out there.  yVPN arose as an attempt to make the freedom I had accessible to all by creating a tool that allows somebody to spin up their own exit node as trivially as connecting to one of the commercial options.

The earliest proof of concept was a handful of bash scripts I wrote in 2018 that I've sadly lost.  The first working app was written in Python and consisted of a [FastAPI backend](https://github.com/bnsmcx/server-yVPN) and a [Typer CLI client](https://github.com/bnsmcx/client-yVPN).  It worked great and I enjoyed learning Poetry to package for PyPi but fundamentally a Linux CLI app really doesn't count as being accessible to the non-technical so I ended up mothballing this to explore another approach.

After realizing that everything should be a web app I started over in Go.  Go was the obvious choice because that's what I'd been working with the most at work and it had become my favorite language.  I've never been particularly fond of frontend work, I struggle to make spreadsheets pretty, so I ended up creating this version using mostly server side rendered static elements with HTMX sprinkled in to get the interactivity I needed.  [This version](https://github.com/bnsmcx/go-yvpn-server) allowed users to setup an account and attach their cloud hosting credentials and spin up wireguard exit nodes.  They could then add clients by scanning a QR code with the Wireguard mobile app, send the config file to a computer, text one to friends or family.  All of that stuff.  It worked great and I had some friends and family using it but this version also eventually was sunsetted.  I think the concept has legs but fundamentally I was more interested in continuing to tinker than figuring out how to make it a business.

[The current version](https://github.com/bnsmcx/yvpn) completely turned the idea on its head.  I'm no longer trying to build something for the non-technical user, I'm building stuff I like to use.  To that end I'm no longer writing it as a web app, not even an HTTP API, instead I'm creating a Bubble Tea Wish app.  I like the idea of not needing to create a client in addition to a server.  I like the idea of not having to maintain an API.  I like the idea of being able to spin exit nodes up and down from anywhere that has an ssh client.  I decided to go with Tailscale because I loved how easily I can expose the new exit node to all my devices at once rather than having to configure each one independently.


I have a lot of thoughts about this concept that I'm letting ferment (percolate?) a little bit but I think the concept is very extensible, in fact I should be able to add support for pretty much anything you can do with cloud-init.  I also have ideas about the paradigms for project support and crowd-sourcing the project's direction could be integrated right into the app.  Suffice to say this is the one that gets most of my bandwidth.

## Alchemy

I'm a huge Neal Stephenson fan and my favorite books of his are [The Baroque Cycle](https://en.wikipedia.org/wiki/The_Baroque_Cycle) and one of my favorite themes of the series is that of Alchemy and how it fit into the evolution of modern chemistry and the enlightenment despite being seemingly at odds with what we consider "good science".  This theme really empowered me to tinker with the alchemy of our time: [trading bots](https://github.com/bnsmcx/solid-eureka).  I didn't manage to turn lead into gold but I learned a ton and can highly recommend taking a stab at it.  Good fun.


## Tree blog

I've always loved the `tree` command in linux.  I love seeing the directory structure.  It inspired me to create [tree blog](https://github.com/bnsmcx/tree_blog) which is a blogging system I wrote in Flask that took it's shape from a directory tree of markdown files.  I even took a stab at my own [markdown to HTML transpiler](https://github.com/bnsmcx/probable-guacamole) though you probably shouldn't use it, there are tons of mainstream options that do it better.

## Hashcat GUI

There was a period during my time as an undergrad where I was fascinated with cracking passwords.  I was on the school's CTF team and cracking password hashes is one of the first thing newbie hackers love to learn.  It truly is satisfying, like feeling the pins *snick* into place on a lock and seeing the cylinder turn.  One of the main tools people use for attacking password hashes is Hashcat and I tinkered around with wrappers for it.  [Hash Master](https://github.com/bnsmcx/hash-master) was a Java GUI that worked but after writing it I realized I'd built something nobody wanted, not even me.  I realized that I preferred using Hashcat in the terminal anyway.  This might have been the beginning of my fascination with terminal apps.

## Misc tinkering

- I created a [pushfight](https://github.com/bnsmcx/terminal-pushfight) game board with Bubble Tea.  Not a full game, just a proof of concept with movement.
- I played with an idea for a [tool](https://github.com/bnsmcx/estimating-tolls) to help estimate tolls.
- I wrote CTF challenge called [teatime](https://github.com/bnsmcx/teatime)
- I created a [webpage](https://github.com/bnsmcx/btc) for my dad's podcast and used the project as an excuse to tinker with programattically generating a webpage from a podcast RSS, it is ugly but the logic was fun to write.
- I spent some time [practicing rust](https://github.com/bnsmcx/rust_practice) from a book.
- I wrote a tool called [descent](https://github.com/bnsmcx/descent) for archaeology.  By that I mean exploring old projects.  Basically you could add a readme in every sub-dir and the tool would recursively pull them all together into a single doc.  There are better ways to do that but I love tinkering.
- I wrote a proof of concept for a friend showing how you could have a device with columns of eight switches which could be mapped to an LCD such that when you toggle the positions of the switches the LCD displays the corresponding ASCII or UTF-8 character. [Code is here](https://github.com/bnsmcx/verbose-waffle).
- I wrote [alien invasion](https://github.com/bnsmcx/alien_invasion) from Python Crash Course when I was laid up with my leg in a cast years ago. 

## 📫 How to reach me
- Email: ben@bnsmcx.com
- LinkedIn: [linkedin.com/in/bnsmcx](https://linkedin.com/in/bnsmcx)

