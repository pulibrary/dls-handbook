# Development Practice

## Selecting an issue

We work from the [Work Cycle
Board](https://app.zenhub.com/workspaces/dls-work-cycle-613924a1df719e0013b678b0/board?repos=98223070).

We also have a [Learning-friendly Board](https://app.zenhub.com/workspaces/dls-learning-friendly-62e046ab829aafbe2d6520b2/board) for members of our team who are focused on training and not working on work cycle issues.

The `ready` column of a given board has issues ordered roughly by priority.
Always assign yourself to an issue before to starting to work on it, and move it
to the `in progress` column.

## Pairing

Our team considers ourselves "pairing-friendly." Several of us very much like to
pair, and we all do pair at least sometimes. We've tried various ways of
formalizing our pairing arrangements in the past. What currently works best is calling
for pairing opportunities at the end of stand-ups and to invite someone to pair with
you if you'd like. Pairing on code-review has also been a helpful practice on occasion.

If a PR is submitted by the pair, they can merge it themselves without code
review. The idea is that code review has happened during the process of
development with a pair. They can still request review if they'd like another
opinion.

Some recommended reading:
* [Slides about pairing best practices](https://docs.google.com/presentation/d/1-PhkB_uSPHrz4-eWI6R9AzLo1fGVWqcxMMdUlAWOvng/edit#slide=id.p)
* [On Pair Programming from martinfowler.com](https://martinfowler.com/articles/on-pair-programming.html#HowToPair)
* [How to get better at pair programming from thoughtbot](https://thoughtbot.com/blog/how-to-get-better-at-pair-programming) 

Checklist for every time you pair:
- [ ] Use an editor where you can both see the outline of the project.
- [ ] Turn on absolute line numbers. 
- [ ] Agree on task, scope, and intention. 
- [ ] Set a timer. Remember to take breaks and swap drivers.
- [ ] Keep the chat going. If you're driving, narrate what you're doing.
- [ ] Use Co-authored-by lines in the commit message (This [.gitmessage](https://github.com/pulibrary/pul-the-hard-way/blob/main/gitmessage.md) file might be handy)
- [ ] Check in afterwards about how it went. 

## Ensembling

Sometimes our team likes to "ensemble," which is all working together at the same time in the same room on a particular feature or ticket. This allows us to quickly distribute knowledge around core parts of our code and design as a group. We see it as a low stress way to collaboratively learn. Our common practices are as follows:

1. When starting an ensemble, have everyone "Roll Initiative" - this is a roll of a 20 sided dice to determine the order of the person typing. You can roll by searching "Roll d20" in Google and reporting the number.
2. Use the "Pomodoro" technique - work for 25 minutes, take a 5 minute break, and then switch the person "driving" (the one typing.)

## Design

A fluid and successful user experience for our patrons is a key requirement of our applications. Our process around design prioritizes iteration, understanding, innovation, and collaboration.

Rather than have a concrete process for all cases, we work with a set of guidelines and tools that we reach for depending on what seems most likely to move us towards a better experience to meet our goals.

In all these cases remember that design is often a personal experience. Feedback and engagement should be collaborative, friendly, and focused on the goals of the experience.

### Design Sprint

**When:** A new project is being started.

**How:** Gather key stakeholders for an intensive week of collaboration. Design activities to gather key goals, success criteria, audience, and core interactions. Some resources:
  * [Thoughtbot Design Playbook](https://thoughtbot.com/playbook/designing)
  * [Gamestorming](https://gamestorming.com/blog/)

**Output:** Various artifacts that will lead towards a successful implementation.

**Examples (likely private):**
  * [Digital Collections](https://drive.google.com/drive/u/1/folders/18X3JoTwYcxPDpUnpAWxmIhJ6LSeJp291)
      - Audience + Problem Statement
      - Audiences
      - Success
      - First Step
      - Metrics & Design

### Success Criteria, Goals

**When:** Designing a new page or experience.

**How:** Discussion or various brainstorming exercises, likely in collaboration with other units and stakeholders.

**Output:** Documentation in the repository about what the goals of a page or new experience are.

**Examples:**
  * [Digital Collections Goals](https://github.com/pulibrary/dpul-collections/blob/main/docs/goals.md#search-results-page)
  * [Digital Collections Success Criteria](https://github.com/pulibrary/dpul-collections/blob/main/docs/success_metrics.md)
  * [Digital Collections Audiences](https://github.com/pulibrary/dpul-collections/blob/main/docs/audience.md)

### Participatory Design

**When:** There's many different ways to reach the goal and developers/stakeholders may see different solutions to the same problem given their unique experience.

**How:** Brainstorming exercises such as [Speedy-Eights](https://thoughtbot.com/playbook/designing/design-sprints/04-diverge-exercises/speedy-eights), [Paper prototypes](https://thoughtbot.com/playbook/designing/design-sprints/04-diverge-exercises/3-step-storyboards) with voting on favorite features, or other activities.

**Output:** A ticket comment summarizing the discussion and next steps. Potentially an implementation ticket.

**Examples:**

  * [Digital Collections Filter Iteration Brainstorming](https://github.com/pulibrary/dpul-collections/issues/1159#issuecomment-4347927635)
  * [Digital Collections Mood Boards](https://drive.google.com/drive/u/1/folders/1lWkptsGVgb6vioVeXXZ81d9RBmGu9QLu)

### Mockups

**When:** There are questions about implementation which may be faster to design than to implement and throw away.

**How:** Whatever method the implementors find easiest, as long as it results in a design for feedback. This may be Photoshop, Figma, or even HTML/CSS. There is often several steps of iteration with feedback in standups, in the channel, on the ticket, or in ensembles. The fidelity of the mockup should be enough to make an implementation ticket actionable. Mockup tickets should follow all our normal best practices for actionable tickets, and often include documentation around edge cases or explicit questions the mockup should attempt to answer. Mockup tickets may lead to implementation tickets that are specified and added to the Work Cycle board in the middle of a cycle.

**Output:** An agreed upon mockup and an implementation ticket. This may result in a Design Decision Record to record why certain decisions were made.

**Example:**
  * [Digital Collections Content Warnings Design](https://github.com/pulibrary/dpul-collections/issues/667)
  * [Digital Collections Content Warnings Implementation](https://github.com/pulibrary/dpul-collections/issues/371)
  * [Digital Collections Filters Design Decision Record](https://github.com/pulibrary/dpul-collections/blob/main/design-decisions/0001-filters.md)
  * [Digital Collections Related Collections Design](https://github.com/pulibrary/dpul-collections/issues/889)

### Iteration & Review

**When:** After an implementation has been in place for a while, you may want to go back and look at the original designs to see if the trade-offs still made sense. It may be that you come up with a new idea and want to try a new design that will better meet the original goals.

**How:** Look at the goals, design, and implementation tickets for a feature. If it looks like there may be iteration to do, create a ticket and try it out. Gather feedback from the team and potentially stakeholders as per our normal process.

**Output:** A ticket or pull request with a new implementation.

**Examples:**

  * [Digital Collections Search Result Cards](https://github.com/pulibrary/dpul-collections/pull/754)
  * [Digital Collections Collection Page Iteration](https://github.com/pulibrary/dpul-collections/pull/1157)
  * [Digital Collections Search Button Design](https://github.com/pulibrary/dpul-collections/pull/1151)

## Submitting code

* Ensure code is arranged in logical, unitary commits unless you want it squash-merged.
* Ensure any new or modified code has test coverage. Many of us practice test-driven development, but at the least a test should be confirmed to be failing before the code change is applied.
* Run Rubocop to enforce code style agreed upon by our team.
* Open a pull request in Github
  * Reference the relevant issues, using [github keywords](https://docs.github.com/en/enterprise/2.16/user/github/managing-your-work-on-github/closing-issues-using-keywords) if the issue will be resolved
* Make adjustments as-needed according to code review.
* If your PR isn't getting reviewed, freely post it in slack.
* If your PR is approved and passes CI checks you may merge your own pull request. Usually this happens when it's reviewed before CI is finished.
* If this code was developed in a pair and passes CI checks, you may merge
without waiting for another reviewer.
* Ensure the issue is closed if no further work is required.

## Reviewing code

* Review other pull requests over the course of the day.
* We generally follow the [Samvera Code Review](https://samvera.github.io/review.html) guidelines
* Ask the author of the code to pair with you on the review if desired / required.

## Dependabot

We have set up our github repositories to use Dependabot, which generates PRs to upgrade dependencies based on security warnings. Based on our experience with these PRs it is important to test a deployment to a staging server before merging them even if the tests are all passing. Also, in some of our projects our tests do not fully cover our javascript code. In those cases when javascript dependencies are updated it can be helpful to do a bit of QA before merging.

If the PR has been open for a while, or you've just merged another PR, use the `@dependabot rebase` comment to trigger a rebase before deploying. This can take a few minutes.
