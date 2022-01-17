# Cloud Providers

Going to try to answer some questions:
- Where is your service running?
- Why not run on a desktop at home?
	- In fact, why not a raspberry pi at home?
- Why not build a data centre?

# Assumptions
- You have some kind of code you need to run to serve customer's needs
- Customers don't run the code themselves but instead talk to your service over the network

# Could I host from my home?
Yes, you could. It's been done, usually as a proof of concept or just because you can.

If you have a machine (a laptop or desktop which stays on all the time) and a broadband connection you theoretically have all you need. A raspberry pi is enough to host a site.
 
However you might run into some problems:
- Your broadband connection likely has very limited upload bandwidth when compared to the requirements of even hundreds of customers trying to connect at once
- The reliability of even a business connection to the home isn't great, it's likely you'd see problems with lost data.
- Your machine might not be able to keep up with all the requests.
- You might see a lot of attempts to attack your network (more than you normally see).
- Your ISP might get very unhappy and cut you off.
- Your power could go, leaving customers with no way to reach your service.
- Service quality would go down if you started streaming Netflix :D

# Could I build a data centre?
Technically you could, but it requires a massive upfront capital requirement, has a long lead time and requires a lot of technical knowledge. Not many companies do this any more (you have to really, really know your market requirements and have a clear model for how much you'd save).

# Could I rent space in a data centre?
Yes, and many companies do. There are different degress of this but you typically rent a section of the data centre (usually measured in racks), bring in your own equipment, plug it in and then plug it into power and network you rent from the data centre.

Some companies still do this, though they typically do it when they have some strong requirement to control the hardware.

This isn't as capital intensive but you still need a lot of technical knowledge and lead times to adapt to new requirements are still very long. You might need to plan racking up new hardware a year out.

A huge factor in owning your own hardware is utilization vs investment vs depreciation. It's very hard to use machines 100% all the time, especially if customer traffic varies. You might see 95% of your traffic in short windows each week, leaving the hard ware idle the rest of the time. This is potentially a huge waste of resources and money.

# So where does cloud fit in?
Cloud providers typically let you rent a slice of a machine in a rack in a data centre. They work by having a huge economy of scale. They'll rack up hundreds of thousands of machines and then rent them out. 

As a customer you can rent what you need, increasing or decreasing as demand requires.  Theoretically this leads to more efficient (and cheaper) hosting, but that takes work to get. The biggest advantage is you can grow and adapt quickly. With a physical data centre you need to either guess your growth and buy way ahead of time, or you need to reject customer traffic when you are overloaded.

Worse, your business model might shift and you suddenly need a massive farm of GPUs for AI or massive storage arrays for data. With physical hardware you're left waiting for someone to ship you hardware, with cloud based compute you can quickly rent new capacity in minutes.

Cloud providers can run out of hardware too, which is it's own type of excitement :)

# So Cloud hosting is perfect?
