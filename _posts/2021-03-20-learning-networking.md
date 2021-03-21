---
title: "Learning networking basics"
description: "Brief adventure in unknown networking land"
layout: post
toc: false
comments: true
image: images/some_folder/your_image.png
hide: false
search_exclude: true
categories: [networking]
metadata_key1: metadata_value1
metadata_key2: metadata_value2
---

I have been coding for a couple of years now, and even managed to get paid for it. However, I have to confess that I have no idea how the internet works.

Yes, really. I don't know how machines communicate with each other through the World Wide Web. It has been bugging me that I don't know this, and today is the day I decide to do something about it.

## tl;dr

For a gentle introduction, check out [this amazing, FREE zine](https://jvns.ca/networking-zine.pdf)
Then proceed to read this book **High Performance Browser Networking**, available for free online [here](https://hpbn.co/)

## Here is what I did:

1. Tried to get information from other blog posts, but they are either too technical or not technical enough, or concepts are explained poorly
2. Googled "best networking book", and this book [Computer Networking: A Top-down Approach](https://www.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149) by _James Kurose et al_ showed up. I remembered seeing people using it in college.
3. Skimmed it, realized that there are so much academic information about every little detail of networking, got discouraged.
4. Found this [amazing, FREE zine](https://jvns.ca/networking-zine.pdf) by [Julia Evans](https://jvns.ca/) explaining networking concepts at the right level of abstraction and right amount of detail. Also the illustrations are so witty! You can check out their other zines [here](https://wizardzines.com/)
   
You will learn in this zine the answer to the question **What happens when your computer connect to a website?** and they explains each step in detail:
Below are the steps and the concepts that you will learn. I'm listing them here for you to do quick `Ctrl + F` to find answer to these concepts.

1. Making DNS requests to go from domain name (like `www.example.com`) to IP address (like 104.28.6.94) : Domain name, IP address, CIDR notation, types of DNS servers (recursive/authoritative), DNS server caching, what `curl` does under the hood, `dig` shell command
2. Using the OS to open a socket: socket types (TCP, raw, UDP or Unix), your `python` script is writing data to the socket, and the socket is splitting this data up into packets to send
3. Establish a TCP connection to the IP address: TCP handshake, what's in the TCP header, SYN, ACK
4. Sending HTTP protocol request: HTTP header, HTTP2 (binary protocol, multiple concurrent requests, have to use TLS encryption)

Then you will learn these extra concepts:
- What a port actually is
- How a packet is put together
- How SSL/TLS works
- Different networking layers
- How packets get sent in a local network (MAC address) 

## Next step

I plan to read this book **High Performance Browser Networking**, available for free online [here](https://hpbn.co/). I found this book while googling networking jargons that I had no clue.
I find the following Amazon Review for this book pretty accurate:

> If you ever took a networking class or read a networking book (e.g. Computer Networking: A Top-down Approach) then you know that networking is a broad subject that covers many topics. As a software engineer developing web applications, many of these topics might not be relevant to your day-to-day work (but nonetheless interesting). Browser networking takes the networking parts that are relevant to software engineers day-to-day and lays them out in a clear and concise manner.
