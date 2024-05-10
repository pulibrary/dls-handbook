# Issue Prioritization and Specification

## Issue Lifecycle

Newly created issues in Github go into a "New Issues" column in Zenhub. These
issues are marked by product owners as "On Deck" when they're prioritized for
work on the next work cycle.

When a work cycle is coming up for a project those issues are migrated to the
"Under Consideration" column in the [work cycle planning
board](https://app.zenhub.com/workspaces/dls-on-deck-61929965c266a00012b5d17f/board?repos=26446857,98223070,49439415,157741631,251438007,414316200).
Those issues are then reviewed during a work cycle planning meeting by the team
and product owner, and if they will be worked on that work cycle are assigned
the "work-cycle" label.

## Sudden Priorities

Issues which severely impact the library staff's ability to work are top
priority, and so able to disrupt
the normal rhythm of work cycles. However, being pulled away from a work cycle
is distracting, expensive, and will likely negatively impact the goals of that
cycle. Therefore, it's important to keep track of when they happen and why
they're important so we can move towards greater cycle stability.

If a "sudden priority" issue comes up, a product owner should do the following:

1. Create the Github issue. Include as much information as possible.
1. Add a "Sudden Priority" justification section. This should include how
   staff's work is being impacted and why there are no suitable workarounds.
   Please also include how urgent the priority is - can it wait a couple
   weeks until the next planning meeting, or must it be done immediately?
1. Add the "sudden-priority" label to the issue.
1. Send a message in Slack to the "digital_library" channel so DLS knows to
   begin acting on the issue.

DLS should then do the following:

1. Ensure the issue is actionable.
1. Give the issue a "work-cycle" label. If it needs to be done ASAP, ping DLS in #digital_library and the DLS Lead will work with you to get it prioritized before the next planning meeting.

The DLS Lead reserves the right to remove the sudden-priority label if they make
a call that the issue is best delayed until the next project work cycle. If they
do so, the issue will be marked as "on-deck" and pinned in the work cycle
planning board.

Example of a sudden priority issue:
[figgy/4811](https://github.com/pulibrary/figgy/issues/4811)

### Review

Sudden priority issues will be reviewed on at least a yearly basis in an effort
to identify the kind of work which has most often pulled us away, and how we
might get ahead of those kinds of problems.

[All Sudden Priority
Issues](https://github.com/search?q=org%3Apulibrary+label%3Asudden-priority&type=Issues&ref=advsearch&l=&l=)

## Writing actionable Issues

Some guidelines follow which make an issue actionable and thus able to be added
to a work cycle. Developers and product owners can use the following to
determine if an issue is "ready."

### Bug issues

* Title is clear and concise
* Expected behavior
* Actual behavior (do we have screenshots, links, browser version if relevant?)
* Steps to replicate
* Clear acceptance criteria: "This issue can be closed when the following is true"
* Impact on user is clear

### Feature issues

* Title is clear and concise
* Description includes a user story: "As a __ I need __ in order to __"
* Provides actual or sample data: Do we have a case to develop and test against?
* Clear acceptance criteria: "This issue can be closed when the following is true"
