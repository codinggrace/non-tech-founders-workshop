# HTTP
* User Agents
	* Can't control a user agent (many stories on the reg of people getting into trouble for curl)
	* Don't trust them!
* Hostname vs path
	* vs query string
	* vs anchor
	* "Single page apps"
* Client vs Server
	* LAMP
	* Self hosted vs SaaS
- Protocol
	- What's a protocol?
- The core component the web is built on
- "HTTP APIs"
- Client vs Server
- User Agents

# What is HTTP?
https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol

HTTP (and the secure form, HTTPS) is probably the most common means of transferring information on the internet. This is the original protocol (along with the document format HTML) Tim Berners-Lee wrote in CERN which formed the basis of the World Wide Web.

When you type something like twitter.com into your browser URL bar it gets magically translated to `http://twitter.com/micktwomey` (or more likely `https://twitter.com/micktwomey`) before being dispatched through the network internals of the browser to Twitter's servers. That `http://` (or `https://`) part is a reference to the protocol, HTTP in this case.

You might also see some older protocols like `ftp://` doing the rounds, but they're very rare these days. The most comomon one you might see is `file://` to refer to local files on your machine. The other kinda protocol is `s3://`, but that's not really a protocol, more of a common way to refer to AWS S3 content.

See also: email uses a mechanism called SMTP (Simple Mail Transfer Protocol).

# URLs
URLs are core to the internet and the web.

# HTTP APIs
You might hear people talking about 

# Advanced: A tiny bit of the HTTP protocol
The HTTP protocol is plain text at its core. You could connect via a terminal to a server and type in a request by hand.

```http
GET /micktwomey HTTP/1.1
```

From the example above, this is asking for the `/micktwomey` bit from the request to `https://twitter.com/micktwomey` above.

The server would spit a fairly lengthy response but the core of it would be something like:

```http
HTTP/1.1 200

<html>
... A bunch of stuff to load twitter
```

# Cookies
# Security
