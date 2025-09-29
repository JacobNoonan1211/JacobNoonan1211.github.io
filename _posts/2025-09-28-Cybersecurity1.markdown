---
layout: post
title: "My First Cybersecurity Journey"
author: "Jacob"
catalog: true
header-img: "img/post-bg-2015.jpg"
header-mask: 0.4
tags:
  - Cybersecurity
---

# My First Cybersecurity Journey

## The First Week

### Hacker's Handbook
I first started out by looking at what my teacher reccomended me to do. First, she gave me a "Hacker's Handbook" pdf that included some general info. Some of this general info included:

* Most common types of attacks and why they happen. They mostly happen because of a lack of security and knowledge about security in a website. 
* Some simple attacks were mentioned, such as SQL injections, modifying session tokens, and changing prices with hidden HTML inputs for cheaper products. 


### Microsoft
I then chose a big cybersecurity attack to take a look at. The hack I decided to look at happened in 2021 and targeted Microsoft's exchange servers. I learned some terms I didn't know before, such as a "zero-day vulnerability." I found [an example](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-26855) of how microsoft documents their attacks.

### Juice Shopping
I found a docker image that would create a fake website I can learn how to "hack" on. It's called OWASP Juice Shop. I first read a little bit about SQL injection, as the first task involved using it. I learned if a SQL query uses concatenation and doesn’t have a sanitizing or validation process, it will be easy to exploit the query’s vulnerabilities. In Juice Shop's login, you can put into the username input field <' or 1=1;> to create a SQL query that looks like "sql = “SELECT id FROM users WHERE user = ‘” + “‘ __or 1-1;__". This closes the quotes after the first where condition which allows the exploiter to modify the SQL query. By using "or 1=1", you can make it so it selects the first user made (usually the administrator), because the SQL query will always come out as true.

![Screenshot](../img/in-post/post-sqlinjection.jpg)

## The Second Week

### Hacker's Handbook
To start off the week, I read part of the Hacker's Handbook again. Here is a quick summary: 
One of the main ways of handling user access is authentication. Authentication is a way of verifying the person on the website is who they claim to be. Some common problems with authentication are attackers guessing usernames/passwords, or bypassing the login function. A session is created for each logged in user and has a unique identifier known as a token (a unique string). Tokens help associate HTTP requests with users. A common vulnerability is logging into another user’s account using a compromised token. Tokens can also be guessed if the string is generated in an unsecure way. Access control uses these mechanisms to identify if a user making a request should be authorized to do so.

There are many ways to handle user input. One way is to “reject known bad.” which is blacklisting a set of strings that might be inputted into HTML fields to exploit the website. This is regarded as the least effective method because you can bypass the blacklisted words by making small adjustments to the input. Another method, “accept known good,” whitelists patterns or literal strings that match non-harmful input. If used correctly, this can be the most effective method. The last method, “sanitization,” sanitizes input in many ways. Sanitizing means removing characters from an input that might be involved in an attack.

### Blog

I started thinking ahead of how I want to make my portfolio/blog look. I was originally thinking of something visually pleasing but also minimal. I wanted to put minimal things on the website, but also make those minimal things really cool. I thought that would create an effect of looking nice, but also not having too much. A website that has minimal components but also has cool animations, colors, and other aspects of the components is the homepage of Zen Browser

### Google Certificate 

Midway through the week, I started looking at the Google Certificate. After careful consideration, I am deciding to take the course. I started a little bit on it, and got some of the modules done.

### Lots more Juice Shopping

For the rest of the week, I decided to work a lot on juice shop. I got a lot of the tasks and challenges done. but needed to use a lot of hints. 

