# Product Owners

We strive for each of our applications to have a product owner (PO). The product
owner is usually a key stakeholder for the application who can collaborate
closely with us to guide development. Documentation of our team's [work cycles](/work_cycles.md) and [technical liaison role](/technical_liaisons.md) should give product owners useful context for this collaboration.

The exact practices of each product owner will vary according to the application and the
individuals themselves. Generally, product owners will work to:

* Maintain a list of the highest priority issues for stakeholders on an ongoing
basis.
  * We recommend keeping track of these either in Github using a list of 10
  "On Deck" labeled issues or using Zenhub to organize these to the top of the
  project board's "Ready" column.
  * The Technical Liaison for your project is available to support the PO in this
  effort.
* Participate during relevant work cycles by attending the planning meeting and
  Friday wrap-up meeting when the PO's application is a focus of the cycle.
* Remain easy to contact on Slack during a relevant work cycle to answer
  questions and give feedback.
  give feedback.
* Bring in DLS developers when discussing new features or potential changes to the
  existing system with stakeholders. Prioritize these conversations when a work
  cycle that can address these is likely to happen soon.

DLS will work to:

* Provide appropriate notice to a PO when a relevant work cycle is upcoming, at
least 1 week before the relevant Cycle Planning meeting (see [work cycles](/work_cycles.md).)
  * If the previous work cycle needs to continue to meet our goals, DLS will
    notify the PO of the delay and adjust the meeting invitations appropriately.
* Ensure planning and wrap-up meeting agendas provide times during which POs can
  expect topics to be focused on their project.
* Triage incoming tickets and bug reports.
* Remain easy to contact on Slack to assist with troubleshooting.

Resources for each application, including technical liaisons and links to repositories and zenhub boards, can be found on the [list of applications](/applications.md).

## What's it like to be a Product Owner (PO) for DLS?

### Intro

Welcome! You're now a member of the team, even if we don't report to the same person. We're going to work together to make sure we understand what the stakeholders and patrons you represent need, how best to meet those needs, and how to prioritize those needs so they get the best result for the amount of time we can dedicate to each project.

DLS has multiple POs and many projects to work on and prioritize concurrently, so we won't be able to work on the project and vision you're responsible for all the time, but with your help we'll be able to make your product as impactful as possible with the resources we do have. To make that happen amidst everything we lean on processes and partnership.

### Tech Liaison Partnership

To make that partnership as smooth as possible, one member of DLS will be identified as a "[technical liaison](/technical_liaisons.md)" - this person is your partner towards making sure that the work we'll eventually undertake on your product is as effective as possible. You've got a breadth of features or bug fixes you want to happen, you and your technical liaison will work together regularly to transform those into [well-specified and actionable tickets](/issues.md#writing-actionable-issues). That might happen in a regular working group meeting, check-ins, or asynchronous communication - whatever works for you! The goal is to give you a direct line to DLS and support for specifying tickets and goals, all to support those tickets representing the best way to meet the root need of your patrons.

### Preparing for a Cycle

Eventually your product will be prioritized - either your needs will be obvious, your liaison will share the impact we could have by working on it, or it will simply be clear that it's the next thing to work on. When that happens our expectation will be that you and your liaison will have prioritized at least ten issues, specified them well enough for us as a team to review and come to a common understanding in a one hour meeting, and thought about who these changes are for and how we'll know when they're done. It might be we need to [design](/development_practice.md#design) a new user experience, do some user testing, or start some research to tell what the ultimate feature will be - documenting that as a ticket we do during the cycle will help us keep that work organized and prioritized.

Cycles are three weeks - one week for planning and spin down from the last cycle and then two for execution. You'll get invited to a [cycle planning](/work_cycles.md#work-cycle-planning) meeting where we'll make sure we all understand when those tickets are successful, a daily [stand-up](/work_cycles.md#standup) to unblock any work, and a [cycle wrap-up](/work_cycles.md#work-cycle-wrap-up) to make sure we're in a spot where we can set things down, ensure what we've shipped is stable, and see if we're ready to move on to the next project.

These three weeks are the time to clear your schedule. A cycle will only be as successful as you're available to answer questions, connect with DLS on Slack, and participate in those meetings. For those three weeks we'll interact with you as a full member of DLS, as you're our teammate in getting these features out and our patrons happy.

### Tips

If you think your product really needs work and it's not getting the time it needs, please bring it up to your liaison or the team lead for DLS. There's a strong community of POs at PUL as well - we encourage you to work together to find impact that crosses boundaries. We're all here on the same mission and it's easy to lose track of in the daily work.

If any part of this process doesn't work for you, talk to DLS. You're a member of the team, and our team's processes should be as effective as possible for all its members. There's a good chance we can adjust things to make sense.

### FAQ

1. How much heads-up will I have that a cycle is coming?
  * We promise at least one week. For many POs that's much too little - we can schedule further out, but it may result in less relevant or immediately impactful work, we can't promise that folks won't be on vacation, and generally we believe that the time to solve impactful problems is when they're impacting our patrons.

1. How do I know a feature will be impactful?
  * Great question! It varies so much it's hard to give a solid answer. We try to make sure our POs can well represent our primary user groups, so it's often the case that it just feels natural - in your every day, what are the things that are bothering your patrons the most? What do you see a lot of, that if it was gone, automated, or made more clear would simplify their (or your) life significantly? We encourage our POs to think broadly here as well - sometimes the most impactful thing is to change where a button goes, but other times it's integration with other products or large new user experiences. You don't have to come up with how to fix it on your own - we're here to help. You know the problems, we'll work together to find the solution and make it reality.

1. The code repository I'm looking at has a huge backlog of tickets, what do I do about that?
  * Feel free to close feature tickets that you're unlikely to prioritize. It's often hard to get past the wall of tickets in a repository built from sheer history, so we encourage you to look at the product with fresh eyes when possible. That backlog may have some good ideas you want to center yourself around, but through your connections with users you'll know what will really make a difference - prioritize those, even if it means making a new ticket, don't feel like you have to do what's in the queue.

1. What about maintenance?
  * The team or the liaison may add maintenance tickets to your cycle - these are generally things like updates to core dependencies or adjustments to match our existing practices. All maintenance work we do is to ensure that feature work can happen as smoothly as possible over a long period - if we didn't do it, then features or updates would start taking longer and longer to implement. If you're looking at a wall of tickets in a cycle that you don't understand, please talk to us - we'll try to talk them out, and it may be that we need another cycle so we can more effectively split maintenance and improvements.

1. We didn't finish a ticket in this cycle, will we finish it later?
  * Often times the team will scope a ticket down to its smallest form so we can get it out in a cycle and see if it works. If it does, we iterate from there - we can always come back and improve something if it's clear it'll have the impact we want. If the feature didn't ship at all, we'll do our best during wrap-up to identify that and come up with a plan to get it shipped. DLS does its best to not leave work half-done - it sits in our hearts as much as it does yours, it's less of a distraction to get it wrapped up than abandoning it, unless it's clear we need to rethink the feature from scratch.

1. I need to get a hold of DLS and my liaison is gone, how do I do that?
  * We're always available on Slack in the #digital_library channel, simply ping us with @dls. We're here to help - the liaison doesn't have to be your only way to talk to us, they're just one guarunteed way to get off-cycle partnership.

1. Do you have any tips on being an effective PO?
  * Not directly, but I'm sure your colleagues do! You can find your PO friends in Slack in the #pul-product-owners channel. They're a great support network who can help you feel comfortable and centered.
