# Phase 2: Observation and Validation (with Gates)

Phase 2 is where we watch to see if the learner did what we asked them to do. With Learning Lab, we are watching for the _event_ to be sent by GitHub and then checking to see if it was the event we were expecting.

The events that are sent to Learning Lab alert Learning Lab that something has happened. But, to create a good learning experience, we should validate that the learner did the right thing. For example, if we ask a learner to commit a function to a file, we'll get an event when they've committed to a branch. But we would receive the same trigger, but they may not have committed to the correct file! In these cases, use a _gate action_ for validation. Gates can:

- Validate that a closed pull request was merged
- Check the contents of a comment or commit with regex
- Ensure an opened issue contains body text

A [:book: `gate`](https://lab.github.com/docs/actions/gate/) is a Learning Lab action. Gates are conditionals, and they behave much like a conditional in Javascript.

You can also get creative here - maybe you want to include tests in the template repository. When the tests are run, the status could be the event that you check.

## Step 10: Write a gate

As an example of how gates work, let's validate the learner's pull request title. This information is accessible to us [:book: from the payload](https://lab.github.com/docs/events#accessing-event-payloads) that is sent with the `pull_request.opened` event. 

You can see an example of all the information sent [in the GitHub Developer docs](https://developer.github.com/v3/activity/events/types/#webhook-payload-example-26).

We'll add the [:book: `left:` option](https://lab.github.com/docs/actions/gate/#options) to the gate, and compare its value to the expected pull request's title.

A completed example of this would look as follows, with comments on the right starting with a hash `#`:
```yaml
actions:
- type: gate                            # using the gate action
  left: '%payload.pull_request.title%'  # get the title from the pull request object inside of the payload
  operator: ===                         # check for strict equality, see more at https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Identity
  right: Add name to README             # this is the expected value
```

### :keyboard: Activity: Write a gate to check the user's first step

1. [Edit the `config.yml` file]({{ url }}) on this branch around line 32.
2. Add a `type: gate` action on line 32.
3. Add a `left:` option to the gate.
4. Set the gate's `left:` option. This could be to the pull request's title (`'%payload.pull_request.title%'`) or some other information from the payload based on the event trigger.
5. Set the gate's `operator:`, usually to `===`.
6. Set the gate's `right:` to the title we expect, like the name of the pull request, or regex for what is expected from the commit contents, or any other amount which makes sense in your case.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>

> Aren't sure what event and gate to use? No worries - you can borrow these:
> ```
> - title: Assign yourself
>   description: Assign the first issue to yourself.
>   translations:
>   event: issues.assigned
>   link: '{{ repoUrl }}/issues/1'
>   actions:
>   - type: gate
>     left: '%payload.assignee.login%'
>     operator: ===
>     right: '%user.username%'
> ```
