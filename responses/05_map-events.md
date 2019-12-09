# Events

Alright - you've gotten a project chosen, and you've laid out the steps for your learners. Next, we're going to get into something new with Learning Lab: events! (You can learn more detail about this in [the documentation](https://lab.github.com/docs/events).)

An `event` is the webhook that the learner triggers, and it's how Learning Lab knows that it should do something. [You can see all of the events in GitHub's documentation](https://developer.github.com/v3/activity/events/types/). Some of the most common examples are `pull_request.synchronize` or `issue.comment`. Next, your job is to map your learning objectives to events.

### Mapping behaviors to events

How can each learning objective or step be translated through a GitHub event? A risk here is to have too many of the same type of events, or to have events represent things that aren't actually what you're trying to teach.

For example, you may want to show a lot of information to the learner, and then have them close the issue to signify they've read it. That may make sense for one or two steps in your course, but imagine going through a whole course like that - it isn't actually checking if the learner read - it's checking if the learner knows how to close issues!

### Event quality

This step will reveal some things about your course, so it's important to pay attention.

Try to choose events that correspond directly to what you want the learner to do. If you're trying to teach the learner to import a `npm` module into a `package.json` file, have the event be the actual commit of the user doing that.

## Step 5: Map learning objectives to events

Remember the steps you wrote earlier? Let's find the corresponding events. You'll see some are already done for the examples, but you can focus on your own.

### :keyboard: Activity: Map the learning objectives you wrote to specific events from GitHub webhooks

1. Take a look through [GitHub's documentation for event triggers](https://developer.github.com/v3/activity/events/types/)
2. Edit the `config.yml` file and make note of the event trigger that matches your first objective

<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
