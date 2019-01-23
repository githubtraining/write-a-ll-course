We need to validate against the learner's pull request title. This information is accessible to us because it is a pull request that triggered this step's execution (specifically, a `pull_request.opened` event).

We'll add the `left:` option to the gate, and set it to the pull request's title.

Activity:
1. Add a `left:` option to the gate
1. Set the gate's `left:` option to the pull request's title which is `'%payload.pull_request.title%'`.
1. Set the gate's `operator:` to `===`
1. Set the gate's `right:` to the title we expect which is `Add name to README`

You can also accept the suggested changes below. They're in batch, so you'll have to go to Files Changed. 