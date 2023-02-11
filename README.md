# http-workshop
## Intro/abstract

My NDC 2023 workshop https://ndcoslo.com/agenda/part-12-artisanal-http-or-http-by-hand-0jfs/0xeiawe0qsu

> In this workshop, we will dig into HTTP 1.1 - the Hypertext Transfer Protocol - from the ground up. We will iterate on the problem of communication between computers, 
> starting by typing text in a terminal on one computer and sending it over TCP/IP to another computer. We will gradually build on this, and before you know it, we are 
> talking to HTTP-savvy programs like browsers. Along the way, we’ll introduce tools such as netcat, curl, jq, wireshark, nginx and k6. Our goal is that you should 
> understand the capabilities of HTTP better, be able to design solutions that use the capabilities of HTTP to its potential - and have new tools and tricks you can use 
> when troubleshooting. The format will be highly interactive, so bring a laptop with a Linux terminal of some sort (For example WSL2 with Ubuntu on Windows, a Mac or a 
> real Linux box). If you would like to do the workshop in a pair, bring a friend - or let us know and we can hook you up with someone. For those that prefer to work 
> alone, it is perfectly fine to talk to your own browser on your own laptop, too.

## Running the workshop/tools
There are a varieties of tools we can use for this workshop, some tools will be considers "must-haves", some are fun to try and optional.
They can be run either in GitHub codespace, as dev containers locally on your laptop or by installing the tools on your linux machine, if you have a Mac it might work, on Windows the only reasonable option is to use WSL2 or a devcontainer. All these options will be decsribed in detail.

### WSL2 / Linux (and likely Mac)
Setup...

### GitHub Codespace
Setup...

### Devcontainer locally on your machine
Setup...

# Assignments
The order is the intended workshop order, but feel free to skip to whatever you find most interesting. 
I use some emojies to indicate if things can be skipped or not.
🧱 is considered a foundation of sort, and should not be skipped. These will be tutorial-ish.
💡 These are good to get better insights, likely include some more thinking/playing around on your own. Can be skipped.
🎓 For extra points and deep-dive, feel free to skip, likely includes more work and things to figure out on your own.


## Part 1 - TCP/IP the foundation
We need to have a basic understanding of the layer underneath us - TCP/IP. TCP/IP is hard to build, but can be simple to use, so it is a great foundation to stand on.
It also provides some motivation for a protocol and understanding of the basic tools.

### 🧱 - Basic chatting with netcat over TCP/IP
This is a must-do. Let's just talk to eachother over HTTP

### 💡Hanging up properly, closing sockets
This is nice, useful to understand how HTTP sockets work and scale and get re-used etc, but not required for the workshop.

### 🎓 Inspecting traffic with tcpdump and/or wireshark.

### 🎓 Chatting to a machine in the cloud
Setting up netcat on a publicly accessible virtual machine. Allow you to talk to multiple users.

### 🎓 Using my HTTP chatbot
Highly experimental software.... 
https://github.com/bjartwolf/http_chatbot

## Part 2 - HTTP basics
### 🧱 Client  - talking to some internetservices
Let's call some web services on the internet and talk to them.


### 🧱 Server
Let's be a server and talk to curl or postman or something.

## Part 3 - Playing with responses
### 🧱 Redirects
Might be some server-sent events etc in here too...
### 🧱 Sending json to a curl client
Let's build modern web API to send JSON to a curl client3


### 💡 Parsing JSON with jq
Sort of the same, but let's learn a little bit of jq, because this is a cute and useful tool. 


## Part 5 - Talking to browsers/HTML/code-on-demand
Might be some server-sent events etc in here too...
### 🧱 Rendering HTML to a browser

### 💡 Redirecting with javascript
Instead of redirecting with 302s like earlier, try to send HTML with a script to redirect using ```window.location = URL```

### Server-sent events

### CORS
How CORS work - by hand.


### 401 and 403s
Maybe do some hand-rolled security
## Part 5 - Talking through proxies
This is where we introduce HTTP proxies, such as nginx.

## Part 6 - Maybe some Azure stuff and other REAL life stuff...
Why not try to run this in a virtual machine behind a public IP?

### PKCE to Azure B2C by hand
This is a useful exercise to understand how to work with real, distributed hypermedia applications by hand... 
https://blog.bjartnes.dev/posts/auth-flow-pkce/

# Background material

A lot of the examples are shown in videos on Twitter and summarized in my https://blog.bjartnes.dev/posts/http-love, and more will come there two. I might find other formats, YouTube etc, to distribute the videos to make it easy to link it to specific assignments/explanations.
