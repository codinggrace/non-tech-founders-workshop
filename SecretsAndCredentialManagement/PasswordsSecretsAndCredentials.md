# Managing your passwords and credentials

***
>   You’re only as secure as your weakest link.
***
* Email (never ever share, you can generally recover passwords here)
* Ticketing system
* Design tools (like figma, adobe suite)
* Collaboration tools (Miro, zoom, etc)
* social media

> Interesting sceal

The email address you use to create  key accounts is something you should never ever share. You can generally recover passwords if you lost them through it.

The best approach to follow with access control is to only give people access to what they need only. And to have a way to remove that access **fast** . 
Even better if you can schedule the access being removed at the end of their contract. This is not only safe for you and your business, it is also safe for them.

Make sure you have in place two things:

* As the business owner, you have the ability to recover whatever you need  **quickly**. For example, for access to company email address, you can simply disable the account and redirect all emails to a suitable alternative.
* Where that isn't possible, that a condition of getting the last payment  is the hand-over of all company assets including arranging hand-over of all passwords like Administrator accounts, passwords to routers and network attached devices i.e. anything the user administers for you and that doesn't have an easy reset mechanism you can use. I would ensure this happens before the last day.


Another important thing that I really hope you are tired of hearing is: don't use the same password anywhere. 

> Why? 

Loss of sensitive data


* When security breaches happen (and they can happen) if you have single use passwords, the risk is to one account, rather than many.
* Can outsiders guess a password with brute force? some places make it very hard to attempt to guess your passwords but it's not always clear where.

## Managing passwords


There are many ways to share access to an online resource. Generally there are ways to have an account per person

It is also possible to share *some* passwords, if you do  use a password manager, such as: LastPass, Dashlane, bitWarden, etc


### Multi Factor Authentication (MFA)

* The main idea here is to find some way to verify that you are you. 
* The same idea of banks verifying a transaction by asking you to confirm something on the bank app or using the bank thingymebob

### Data breach

This is definitely something you want to avoid. If it happens the solutions is highly contextual. Not only it depends what is was breached but 

* Who (people and organisations) do you need to notify?
* How are you stopping the problem from happening again? 
* Do you need to stop trading while this problem is being solved?


### Single Sign On (SSO)

The idea here is that as long as you are signed in to 1 thing such as your computer or your email, it gives access to other services.

## Critical company secrets (AWS, DNS, GitHub admin credentials)

### AWS and other cloud providers

* Can create other accounts completely free for management.
* Get familiar with the process of setting up a root account and understanding the basics of identity management. 
* Similar principles apply for other similar tooling

#### Guidelines & Best practices

* Don't use the root account except for account setup
* 1 person = 1 aws  user
* Assign users to groups and assign permissions to groups
* NEVER SHARE IAM USERS AND ACCESS KEYS
* Create a strong password policy
* Use and **enforce** MFA 
* Use roles for giving permissions to services
* Use access keys for programmatic access 
* Audit permissions 


## Github and other source control management tools

1. Tightly Control Access

    * Never let users share GitHub accounts/passwords.
    * Require 2-factor-authentication on every contributor’s GitHub account.
    * Any laptops/devices with access to your source code must be properly secured.
    * Repository administrators should manage team access to data. Only give contributors access to the data they need to do their work.
    * GitHub accounts are often personal ones, and do not naturally disappear when users leave the company. Make sure you diligently revoke access from users who are no longer working with you.
2. Never store credentials as code/config in GitHub. There is good tooling to support this for all platforms.


[Convert your github user to an organisation](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-user-account-settings/converting-a-user-into-an-organization)

# Web hosting and domain management

This is the most in some ways the hardest one to give good guidance to because what this looks like widely changes depending on what you use to buy your domain. 
Many low code solutions (wordpress, wix, etc) offer this as an integrated facility

