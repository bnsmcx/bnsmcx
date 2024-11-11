# Hi, I'm Ben Simcox 👋

I’m a software engineer focused on backend Go development. Below is an overview of my public work on GitHub, showcasing everything from quick experiments to more substantial projects. Hopefully, it gives you a sense of who I am as a developer.

## yVPN

I’ve developed a series of VPN management tools, all named **yVPN** (short for "your VPN"). yVPN started as a way to make it easier for me to spin up VPN servers on Digital Ocean. For years, I’d manually set up OpenVPN on a Droplet, which was simple and cheap. But I realized my non-technical friends and family were stuck with commercial solutions. That’s when I decided to build yVPN—a tool that makes creating a personal VPN as easy as using a commercial service.

The first version was a Python app with a [FastAPI backend](https://github.com/bnsmcx/server-yVPN) and a [Typer CLI client](https://github.com/bnsmcx/client-yVPN). It worked well but was still a Linux-only CLI tool—great for me, but not so much for non-technical users, so I abandoned it.

I then rewrote it in Go as a web app with server-side rendered elements and [HTMX](https://htmx.org/) for interactivity. The [Go version](https://github.com/bnsmcx/go-yvpn-server) allowed users to easily spin up WireGuard exit nodes, configure clients, and share VPN access with friends and family. But again, I ended up shelving this version, more interested in tinkering than building a business.

Now, I’ve shifted the approach entirely. The [current version](https://github.com/bnsmcx/yvpn) is built as a Bubble Tea-based TUI, focused on a command-line experience I enjoy using. It’s not a web app or HTTP API—just a TUI that can spin up exit nodes anywhere with an SSH client. I’m using Tailscale to expose the nodes across all my devices seamlessly. This project is still evolving, and I see a lot of potential, including adding support for deploying more than just VPN exits and ideas for crowd-sourced project direction. This gets most of my bandwidth right now.

## Alchemy

As a huge Neal Stephenson fan, I love the theme of alchemy in *The Baroque Cycle*. Inspired by this, I dove into the modern-day "alchemy" of building trading bots. Though I didn’t turn lead into gold, I learned a lot while creating [Solid Eureka](https://github.com/bnsmcx/solid-eureka). Trading bots are a fun challenge, and I highly recommend trying it out.

## Tree Blog

I’ve always loved the `tree` command in Linux for its ability to visualize directory structures. This inspired me to build [Tree Blog](https://github.com/bnsmcx/tree_blog), a blogging system in Flask that uses a directory tree of markdown files. I also wrote my own [markdown-to-HTML transpiler](https://github.com/bnsmcx/probable-guacamole), though you’re better off using established tools for this!

## Hashcat GUI

Back in my undergrad days on the school's CTF team I was fascinated by cracking passwords. I worked with Hashcat and built a [Java GUI wrapper](https://github.com/bnsmcx/hash-master). After completing it, I realized I’d built something nobody really wanted—myself included! A GUI wrapper for a terminal tool when I prefer terminal tools over GUIs!

## Misc Tinkering

- Built a [Pushfight](https://github.com/bnsmcx/terminal-pushfight) game board with Bubble Tea as a proof of concept.
- Created a [tool](https://github.com/bnsmcx/estimating-tolls) for estimating toll costs.
- Developed a CTF challenge called [Teatime](https://github.com/bnsmcx/teatime).
- Wrote a [webpage](https://github.com/bnsmcx/btc) for my dad's podcast, tinkering with programmatically generating a page from a podcast RSS feed.
- Spent time [practicing Rust](https://github.com/bnsmcx/rust_practice) using a book.
- Built a tool called [Descent](https://github.com/bnsmcx/descent) to explore old projects by recursively compiling README files into a single document.
- Developed a proof of concept for a device with 8-position switches that map to an LCD displaying ASCII/UTF-8 characters—[code here](https://github.com/bnsmcx/verbose-waffle).
- Created a game called [Alien Invasion](https://github.com/bnsmcx/alien_invasion) from *Python Crash Course* during an unfortunate leg injury.

## 📫 How to Reach Me

- Email: ben@bnsmcx.com
- LinkedIn: [linkedin.com/in/bnsmcx](https://linkedin.com/in/bnsmcx)

