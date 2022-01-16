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
HTTP (and the secure form, HTTPS) is probably the most common means of transferring information on the internet. This is the original protocol (along with the document format HTML) Tim Berners-Lee wrote in CERN which formed the basis of the World Wide Web.

When you type something like twitter.com into your browser URL bar it gets magically translated to http://twitter.com/ (or more likely https://twitter.com/) before being dispatched through the network internals of the browser to Twitter's servers. That `http://` (or `https://`) part is a reference to the protocol, HTTP in this case.

You might also see some older protocols like `ftp://` doing the rounds, but they're very rare these days. The most comomon one you might see is `file://` to refer to local files on your machine. The other kinda protocol is `s3://`, but that's not really a protocol, more of a common way to refer to AWS S3 content.

# URLs
- URLs are core to the internet and the web.