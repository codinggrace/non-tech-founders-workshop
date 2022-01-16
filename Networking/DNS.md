# DNS

* Core to the internet
* Frequently the cause of many outages
* Frequently misunderstood
* Managing your own domain
	* Why it's important
		* Controls access to everything
		* Often used for verification of ownership
	* Protecting it


# How DNS Works, the 10,000m View

When you or an application wants to convert a human readable name (e.g. facebook.com or mail.google.com) into something the network can use to make a connection to another machine it uses DNS.

Your application typically asks the device it's running on (IOT, mobile phone, desktop, server) to make this lookup. In turn the device will ask a set of servers it's pre-configured to use. These servers in turn might start having to talk to other servers but eventually they should come back with an answer. However the answer might be "not found".

![[DNS Lookup Failure Example.png]]

# How DNS is Structured
DNS is structured like as file system of folders. You read from right to left.

For example mysite.example.com and myothersite.example.com could be read as:
- com/
	- example/
		- mysite
		- myothersite

At different levels different companies "own" the names.

## Pro-Tip: You can use a tool called "whois" to lookup information



# Types of Security Issues
Examples of some seen attacks
- Typo squatting
	- A very simple attack, you buy a typo'd version of a common domain and create a fake site to trick people into giving you credentials or some other information.
	- e.g. goolge.com vs google.com
	- 
- DNS Spoofing
- 