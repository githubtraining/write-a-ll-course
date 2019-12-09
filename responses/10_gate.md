  # 9.3
    # Nice work!


  # 10.1
    # Phase 2 is already decided for us because the _event_ itself is the opening of an issue. If a user can make that trigger, they've learned what we wanted them to learn!
    # In some cases, you may want to use a _gate action_ to validate things. Gates are like:
    # You can also get creative here - maybe you want to have tests be included in the template repository, and then when they're run, the status could be the event, or something that you check. 
    # For now, even though the event itself will give us a pretty good idea, let's say we wanted to make sure that the new issue was opened with a title and with a body, so it's following good communication practices.
    # That gate would look like:
    # Now, add a gate to this step.

```

### Validation

The events that can act as triggers help Learning Lab know when something happens. However, sometimes knowing it happened isn't enough. For example, if we ask a learner to commit a function to a file, we'll get a trigger that they've committed to a branch. But we would receive the same trigger, even if they committed to a different file!

Course authors can use **gates** to be validate the user's completion of a step. A [:book: `gate`](https://lab.github.com/docs/actions/gate/) is a Learning Lab action. Gates are conditionals, and they behave much like a conditional in Javascript. Let's add a `gate`, we'll specify its options in a later step.

## Step 11: Add a gate

Let's now validate the learner's pull request. We asked them to title the pull request "Add name to README" so that's what we need to validate against.

### :keyboard: Activity: Adding a gate

1. Add a gate or accept the suggested change below


```

```

### Step 12: Add validation
We need to validate against the learner's pull request title. This information is accessible to us [:book: from the payload](https://lab.github.com/docs/events#accessing-event-payloads) that is sent with the event. In this case, the information was sent from a `pull_request.opened` event.

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
## Step 10: Write a gate

### :keyboard: Activity: Write a gate to check the user's first step

1. Add a `left:` option to the gate
1. Set the gate's `left:` option to the pull request's title which is `'%payload.pull_request.title%'`
1. Set the gate's `operator:` to `===`
1. Set the gate's `right:` to the title we expect which is `Add name to README`

You can also accept the suggested changes below. To accept as a batch, go to the **Files changed** tab.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>


```

<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
