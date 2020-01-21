# Outline the remaining steps

It is very important to choose events that correlate as directly as possible to what you're asking the learner to do. If you're not using gates* or other tests, the event _should_ be what you're asking the learner to do.

One way to do this is to structure events using dot notation. For example, you could use an event called `issue_comment`. This means Learning Lab would be looking for any event related to an issue_comment, like created, edited, or deleted. But, you could also be more specific in the event description with dot notation. If you use `issue_comment.created`, Learning Lab will only move on if the event is a newly created issue comment.

>_*Gates are an action within Learning Lab that allow you to use logic and verify the learner's behavior. We'll learn more about this later!

## Step 6: Create an outline of learning objectives as events

Go ahead and put in the events for the rest of the learning objectives. You can use this time to re-order them in a way that makes sense to you for a flow of a course.

### :keyboard: Activity: Using the same strategy of mapping learning objectives to events, create an outline of events for your course

1. [Edit the `config.yml` file]({{ url }}) on lines 36, 43, 50, and 57.
2. Map the rest of your learning objectives to [GitHub Events](https://developer.github.com/v3/activity/events/types/).

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
