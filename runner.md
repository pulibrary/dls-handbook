# Runner

Each week a person from the team volunteers to be the "runner." This person
watches [honeybadger](https://app.honeybadger.io/projects) for all our projects
and ensures that newly discovered errors are appropriately ticketed and followed
through on.

## Why do we have a runner?

Our team found that without someone specifically designated to track exceptions
in our application that the rate of exceptions would only go up. By creating
tickets and designating priority issues for the team to work on we hope to
create more stable software for our users.

## How to be the Runner

Running happens on a weekly cycle. There is a new runner every week and the goal
of the runner is to ensure that exceptions which come in have actionable
tickets with sufficient information to close them without honeybadger history.

### Friday Before

Volunteer to be the runner at stand-up or the work cycle wrap-up.

Ensure your notifications are on for all of DLS'
[applications](/applications.md).

### Each Morning

Look through new errors from the weekend or night before. For any that have no
tickets create a ticket with enough of a backtrace to tell what's going on, a
descriptive title of what caused the error, and any background information that
might help work it. Apply the "maintenance / research" label so it appears in
the inbox of our [maintenance
board](https://app.zenhub.com/workspaces/dls-maintenance--research-6139264d4f68940016d4b7cf/board?repos=26446857,98223070,49439415,157741631,27400037,251438007,387577615,404487342).

### When a new error comes in

Do the same as above, but notify #incident_reports if it's indicative of a major
issue that needs immediate response.

### Friday During

Choose one ticket that you either created or saw repeatedly to be worked on
during maintenance/research week. Mark it "high-priority" by clicking the pin in
the maintenance board and mention it at stand-up.

## Runner Support

Running is exhausting and distracting. Don't volunteer too often and lean on
your team when you need support. If, for example, a downtime event leads to too
many errors to get through while keeping up with what you're working on you can
always ask in #dls to split the workload. We're here for you, thank you for
volunteering!

## Errors of certain kinds

1. Staging errors are often due to development / testing. But it could be an
   opportunity to catch an error before we see it in production. If you're not
   sure, check in with the team.
2. Errors that look like attack probes should be ticketed in princeton_ansible
   for lack of a better place. Operations will use them to look at Signal
   Sciences configuration.
3. Errors that look like SIGHUP from closing a console on a box can be set to
   "ignore".
