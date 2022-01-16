# DNS

* Core to the internet
* Frequently the cause of many outages
* Frequently misunderstood
* Managing your own domain
	* Why it's important
		* Controls access to everything
		* Often used for verification of ownership
	* Protecting it

# What is DNS?
The Domain Name System (DNS) is a mechanism to identify machines on networks, be they private networks or the internet. It's often called a "phone book" for looking up unique identifying addresses for machines.

# Why is DNS Important?
DNS is pretty much the only way a device can figure out how to connect to a service. It drives web browsers and all services applications use. It's used for machine to machine communication within a company. 


# How DNS Works, the 10,000m View

When you or an application wants to convert a human readable name (e.g. facebook.com or mail.google.com) into something the network can use to make a connection to another machine it uses DNS.

Your application typically asks the device it's running on (IOT, mobile phone, desktop, server) to make this lookup. In turn the device will ask a set of servers it's pre-configured to use. These servers in turn might start having to talk to other servers but eventually they should come back with an answer. However the answer might be "not found".

![[DNS Lookup Failure Example.png]]

An example lookup might be something like `www.codinggrace.com` which might map to two underlying machine addresses, `172.67.134.3` and `104.21.25.104`.

# How DNS is Structured
DNS is structured like as file system of folders. You read from right to left.

For example mysite.example.com and myothersite.example.com could be read as:
- com/
	- example/
		- mysite
		- myothersite

At different levels different companies "own" the names.

## Buying a Domain
When you "buy" a domain you are typically leasing rights to it for a period of time (usually a year). You typically buy domains from registrars like Gandi.

If you don't keep paying for the domain it typically "lapses". This means it becomes available again for anyone in the world to purchase.

### Security Issue: Buying a lapsed domain
A simple and effective attack is to buy a domain a company has forgotten to renew. Even big companies fall foul of this.

Once you've bought the domain you can redirect any traffic you wish to your own servers.

Typically the original company can dispute this and reclaim ownership of the domain but this can take time.

## What Does Owning a Domain Get You?
In a nutshell owning a domain like `example.com` gives you full control over where traffic for `example.com` goes, as well as all "sub-domains" like `www.example.com` or `www.another.example.com` goes to. 

## What Does Owning a Domain Not Give You?
- A domain simply gives you a means to map addresses
- It will not give you any hosting or content, but many domain registrars offer this as well

## Advanced: You can use a tool called "whois" to lookup information

`whois` is a tool which allows you to query a database of all registered domains. Useful for looking up ownership and where to send complaints (domains must have a complaints address).

It can be run from command line (On a mac run `Terminal` and then type `whois somedeomain`) or from some websites. e.g. https://network-tools.com/whois/ offers free whois lookups.

#tools/whois

# Types of Security Issues
Examples of some seen attacks
- Typo squatting
	- A very simple attack, you buy a typo'd version of a common domain and create a fake site to trick people into giving you credentials or some other information.
	- e.g. goolge.com vs google.com
	- 
- DNS Spoofing
- 