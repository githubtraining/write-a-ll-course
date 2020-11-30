# Config logic

To put this response in the config, it will be very similar to phase 1. But, _where_ the action goes is different. We need to be careful of the gate here. If the gate fails, we can have special logic for the "unhappy path" response. The "happy path" response will be a regular response triggered if the gate is successful, like:

```
- type: gate
    left: '%payload.pull_request.base.ref%'
    operator: ===
    right: main
    else:
    - type: respond
      with: 01_try-again.md
- type: respond
  with: 01_nice-work.md
```

## Step 12: Write the config logic

Go ahead and edit the config to add the unhappy path _and_ the happy path response.

_Are you noticing that we're asking a bit more of you now? Since you've already added a response before, we're now asking you to do two at a time. This is on purpose - it's important to balance how much you're asking learners to do. It's bad to bore them, but it's also really bad to overwhelm them. Every learner is different, so try to pick a "middle of the road" solution. This is ours. What do you think?_

### :keyboard: Activity: Write the config logic for both responses to the learner in their first step

1. [Edit the config file]({{ url }}) in this pull request to include the logic for both responses around the gate.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
