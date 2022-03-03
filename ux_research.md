# Evaluating and Improving User Experience in DLS Applications

## What is User Experience?
When we talk about User Experience, we are talking about all aspects of the end user’s interaction with our organization, its services, and its products.

The first requirement for an exemplary user experience is to meet the exact needs of the patron, as intuitively as possible. The second requirement is simple and elegant design that produces products that are a joy to use.

True user experience goes far beyond giving users what they say they want, or providing a checklist of features. In order to achieve high-quality user experience in our offerings there must be a seamless merging of the services of multiple disciplines, including software development, communications, and interface design.

Because the sources of UX issues can exist across departments, it’s important to note that our team may at times have to lobby for changes to be made in other peer team applications, departmental policies, communications, and more. In such cases we should present evidence to back up our change requests. One of the most effective ways to persuade others that there is a problem that needs fixing is to show them the users as they struggle to complete their goals. This approach evokes empathy in the viewer and is more likely to convince a stakeholder that a change is necessary than a logical argument.

## What is Usability?
Usability is a quality attribute that assesses how easy user interfaces are to use. The word "usability" also refers to methods for improving ease-of-use during the design process.

Usability is defined by 5 quality components:

- **Learnability**: How easy is it for users to accomplish basic tasks the first time they encounter the design?
- **Efficiency**: Once users have learned the design, how quickly can they perform tasks?
- **Memorability**: When users return to the design after a period of not using it, how easily can they reestablish proficiency?
- **Errors**: How many errors do users make, how severe are these errors, and how easily can they recover from the errors?
- **Satisfaction**: How pleasant is it to use the design?

There are many other important quality attributes. Another key one is utility, which refers to the design's functionality: Does it do what users need?

In DLS, we want to determine if something we are working on is Useful. Usability and Utility are equally important and together determine whether something is useful. Something that is easy to use, but not what you want is not useful. It's also no good if the system can hypothetically do what you want, but you can't make it happen because the user interface is too difficult. To study a design's utility, we can use the same user research methods that improve usability.

- **Definition of Utility** = whether it provides the features you need.
- **Definition of Usability** = how easy & pleasant these features are to use.
- **Definition of Useful** = usability + utility.

# How to Improve Usefulness?

## Measuring Usability
We can't improve what we are not measuring. We measure the usability of apps and features by keeping track of how many tasks users are able to complete and how easy it is for them to complete the tasks. This will allow us to track our most and least usable systems, measure improvements, and help us prioritize UX work.

We will want to include tasks that were used in past testing scripts if we have reason to believe the  experience has changed. By re-testing previous tasks, we can measure how effective (or not) our improvements are.

## Usability Testing
We test usability for the purpose of improving our software systems and interfaces. Our goal is to learn as much as we can about how useful our software is with as little overhead as possible, so we lean towards a less formal testing process. All data collected is used internally, and because DLS has no intention of publishing the findings, we do not have to obtain the approval of an Institutional Review Board (IRB).

There are many methods for studying usability, but the most basic and useful is Usability Testing, which is comprised of the following effort:

- [ ] Determine the top 1-3 user goals for the application you're testing.
- [ ] Determine what else the research team would like to learn from a round of usability testing.
- [ ] Gather tasks from previous rounds of testing to determine if recent work on improving the experience has been effective.
- [ ] Script tasks for the user to complete during the test session based on the objectives in previous three  checkboxes.
- [ ] Recruit and schedule representative users.
- [ ] Ask users to complete representative tasks with the design.
- [ ] Observe (and sometimes record) what the users do, where they succeed, and where they have difficulties with the user interface. The only interaction we should have with the user is to ask them to complete a task, or ask them to describe their thinking and reasoning out loud as they interact with the UI to work through the task.
- [ ] Review recordings and notes to document which tasks were completed or not completed. Make notes of why the user may have failed to finish each incomplete task.
- [ ] Write a report summarizing issues encountered and file in the GDrive Project Folder for Usability Tests.
- [ ] Create GitHub tickets for interface issues identified in the report. Tag the issue with the _User Experience_ label. Suggest solutions in the discussion section of the issue.
- [ ] If the team needs stakeholder approval to alter a UI piece, or to implement a preferred solution, create a "highlight reel" to share with stakeholders demonstrating the users' frustrations so stakeholders better understand the issue and empathize with the user.
- [ ] Determine the preferred solution as a team.
- [ ] Implement preferred solution.
- [ ] Re-test during the next Usability Testing cycle to ensure the change improves users ability to complete the task.

It's important to test users individually and let them solve any problems on their own. If we help them or direct their attention to any particular part of the screen, we have contaminated the test results.

To identify a design's most important usability problems, [testing 5 unique users](https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/) is typically enough. It's a better use of resources to run many small tests and revise the design between each one so we can fix the usability flaws as we identify them, rather than scheduling one or two big expensive studies each year. Iterative design is the best way to increase the quality of user experience. The more versions and interface ideas you test with users, the better. Finally, listening to what people say is often misleading: you have to watch what they actually do.

### Recruiting and Screening Research Candidates

Although there are many ways to recruit test candidates, at DLS we have two available to us, maintaining a pool of volunteers and "hallway recruiting". No matter which method is selected for a project, make sure to disclose that we intend to record the test session before scheduling. If a prospective participant is not comfortable with being recorded, it would be best to find another participant.

#### Pool of existing participants

It makes sense for us to recruit from our existing users and staff to establish a pool of volunteers who are willing to either try out new features or participate in research opportunities in general. One challenge our team faces is that we are not able to compensate these testers for their labor. To remedy this problem, we can look to the large pool of staff and student workers who are presently compensated for the tasks they are asked to perform at the Library, and perhaps even collaborate to establish a network of potential test candidates at the University. We will need the permission from PUL leadership to pursue this method of recruitment. Using a pool of existing participants is best for more formal testing of a larger set of tasks.

There is also the cost of creating a pool of participants and maintaining it, as well as doing the work of scheduling and coordinating participants. There might also be some sampling and confirmation bias due to participants’ existing knowledge of certain systems, so we may have to do some simple screening of candidates to counter this.

The results of these tests should generally be private, so we don’t need to perform an IRB review.

#### Intercept studies (or "hallway recruiting")

Intercept studies are useful for getting quick feedback on a feature or interface. A group of 5-10 users should be sufficient for this type of testing. The basic idea is simply to approach people in the building (or for remote folks, reach out to University contacts via Slack) and ask “Would you be willing to take 5 minutes to participate in a quick survey?”

These types of studies can be done virtually (via Zoom) or in person (in the lobby, office hallway, or coffee shop). They are ideal for quick feedback on a small subset of features.

### Scripting Task Scenarios
Before scripting tasks for the participant to complete during testing, you need to be clear on two things. First you will want to ask the participant to achieve the most important goals the site enables. Second, you will want to know what you want to learn from this test and make sure your tasks cover those use cases. For example, a new feature may not enable the completion of the most important goals, but we still want to make sure that it works as anticipated.

When scripting [representative task scenarios](https://www.nngroup.com/articles/task-scenarios-usability-testing/) for the users to complete, make sure to provide the participant with all the information that she needs to complete a task, without telling her where to click. During a usability test, mimic the real world as much as possible. Recruit representative users and ensure that each task scenario: is realistic and typical for how people actually use the system when they are on their own time, doing their own activities encourages users to interact with the interface
doesn’t give away the answer.

### Recording Observations
It’s important to capture test sessions for future analysis, comparison, and evidence. To ensure that the relevant information is captured, we recommend the participation of a facilitator and a notetaker (in addition to the test participant) for each session to save time and allow for smooth transitions between tasks.
For anything other than the most casual intercept studies, we should record each session as it captures the most evidence for building an argument for change. For this reason, participants must provide consent for us to record them. The best way to do this is to read the user a consent form ([sample](https://docs.google.com/document/d/1S2E1QbVDIhCjc8UOrurdP8aus3r06WMHDuR1d_HNcNs/edit?usp=sharing)) and ask them for their consent to the terms on camera. This approach ensures that their consent stays with the recording and does not get lost.

Each test will produce a set of artifacts. Typical artifacts are test scripts, score cards, session videos, transcripts, and recommendation reports. For any applications or features that require significant changes to fix, it is helpful to compile a “summary reel” that highlights user failures and can be shared with stakeholders to demonstrate evidence of the problem.
Testing artifacts should be well organized and live in the following path: [GDrive > DLS > Project Supporting Materials > {Project name} > UX Artifacts > {Date of Test + Feature Tested}](https://drive.google.com/drive/u/1/folders/1S671v6VEBfKaXPI2eSesEDSmEbCQ4f4s).

We have typically not shared anything but video summaries and recommendation reports outside of the project team. Wording should be included in the consent terms that allows us to share test data and artifacts outside the team, but still within the Library, when another team has the sole  authority to modify the problematic components of the system.

## Using FAQs and User Manuals to Identify UX issues

If an application is not very useful, users will often ask the librarians and public services staff questions about how to accomplish their goals. These often end up in lists of Frequently Asked Questions on a website or application, which may provide temporary relief for users and public services staff, but highlights poor design. FAQs can be useful in determining an application’s most important representative tasks that are the most challenging for users.

## More UX Methods and Activities
The chart below describes UX methods and activities available in various project stages. This image is produced by the Nielsen Norman Group which also provides [a good overview on when and why to use each method](https://www.nngroup.com/articles/which-ux-research-methods/).
