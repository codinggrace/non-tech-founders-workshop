# Overview
* How marketing can cause security incidents
* Why you sometimes get funny looks when asking for something simple
* Very coupled to cloud providers
* How to achieve some goals
* "KISS"


Examples:
- When a domain registrar offers to "park" your domain what are they doing?
- When "redirecting" traffic what different means of doing this are there?
- When you ask someone to redirect `www.mycompany.com/big-conference` to `big-conference.mycompany.com` what are you asking for? And vice-versa?

# How DNS and HTTP Relate

1. When you or an application make a request to `https://www.example.com/some/page` there are a two main parts to this request:
	1. The bit after the `https://` bit, but before the first `/` is the hostname portion. This hostname is the machine (or server) you want to talk to. DNS is used with this hostname to lookup a machine friendly name. Then a connection is made to that machine.
	2. The portion 

Other parts of the request:
1. There might be a `?something=else&another=thing` portion of the URL. 