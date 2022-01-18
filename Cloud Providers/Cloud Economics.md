# Cloud Economics

This topic rapidly comes to dominate over every other topic (infrastructure design, deployments, engineering choices) as cost of different design decisions has a large bearing on success.

# Overly Simple Example
If you run 100 m5.large EC2 instances constantly it might cost 8,831.89 USD per month.

If you re-engineer the workload to run on identical instances but using AWS's spot instance model you could instead pay 3,676.63 USD per month.

The choice to re-engineer doesn't come without cost but (engineering resources and opportunity cost) but might significantly move the needle.

This is a very simple example. AWS is considered one of the most complicated cloud providers when it comes to pricing, it can be very hard to predict costs without sophisticated analysis.

# Sometimes Simple Choices are Effective
In AWS you nearly always want to start looking at Compute Savings plan options (and their related options like reservations).

A simple compute savings plan for the above much cost 35,916.00 USD up front for 1 year but reduce monthly cost to 4,013.89 USD with no engineering work at all (equivalent to 2,993 + 4,013 = 7,006 USD per month). A full up front payment might be 70956.00 USD (equivalent to 5,913 USD per month)

Even better, these savings tend to transfer, so changing and adapting workloads will quite often keep the savings.

There are also EC2 savings plans where you commit to a monthly spend in return for savings (e.g. committing to spending 4891.00 USD per month for the above for a year).
