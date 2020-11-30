# Events

Alright - you've chosen a project, and you've laid out the steps for your learners. Next, we're going to get into something new with Learning Lab: events! (You can learn more about events in [the documentation](https://lab.github.com/docs/events).)

An `event` is the webhook that is triggered when the learner does something in their repository. Every webhook for the learner's repository is sent to Learning Lab. These events are "read" by Learning Lab. If it is the event the bot has been waiting for, the bot will do what you command. Otherwise, it will ignore the event.  [You can see all of the events in GitHub's documentation](https://developer.github.com/v3/activity/events/types/). Some of the most common examples are `pull_request.synchronize` or `issue.comment`. 

### Map behaviors to events

How can each step translate to a GitHub event? Having too many of the same event may be a bad signal. Make sure that events represent things that you're trying to teach.

For example, you may want to show a lot of information to the learner, and then have them close the issue to signify they've read it. That may make sense for one or two steps in your course. But, imagine going through a whole course like that. It isn't actually checking if the learner read - it's checking if the learner knows how to close issues!

### Choose the right events

Try to choose events that correspond directly to what you want the learner to do. If you're trying to teach the learner to import a `npm` module into a `package.json` file, that commit should be the event.

| Behavior | Events |
| ------------- | ------------- |
| What can I observe that confirms the user demonstrated the skill or knowledge? | What event triggers are available through GitHub? |
| Write a function (commit) | [`pull_request.synchronize`](https://developer.github.com/v3/activity/events/types/#pullrequestevent) |
| Solve a merge conflict (commit) | [`push`](https://developer.github.com/v3/activity/events/types/#pushevent) |
| Open a pull request | [`pull_request`](https://developer.github.com/v3/activity/events/types/#pullrequestevent) |
| Implement a test | [`status`](https://developer.github.com/v3/activity/events/types/#statusevent) |
| Comment on an issue | [`issue_commented.created`](https://developer.github.com/v3/activity/events/types/#issuecommentevent) |

## Step 5: Map learning objectives to events

Next, your job is to map your learning objectives to events.

Remember the steps you wrote earlier? Let's find the corresponding events. You'll see some are already done for the examples, but you can focus on your own.

### :keyboard: Activity: Map the learning objectives you wrote to specific events from GitHub webhooks

1. Take a look through [GitHub's documentation for event triggers](https://developer.github.com/v3/activity/events/types/).
2. [Edit the `config.yml` file]({{ url }}) on line 29 and make note of the event trigger that matches your first objective.

> Not sure where to start? Use some of the events in the table above to get started!

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
