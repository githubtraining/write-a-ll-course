# Learning Lab Actions

Awesome! You're probably thinking - how is Learning Lab validating that I did the thing just now!? And you have a point. With text, it's tricky - so I checked to make sure you wrote more than 5 words, but I'm not checking to see if you wrote anything that makes sense. This is a limitation of Learning Lab.

For now, here are a couple examples of real, human-proofed answers. Compare your answer and notice - is yours similar? Is it very different? What would you change?

- Link
- Link
- Link

### Action `type: respond`

We need to figure out _how_ to say it to the user in Learning Lab. Now is the time to learn about _actions_. Actions are reusable modules that each course has access to. They are each designed to do very specific things, and nothing more. This is to optimize for reusability and simplicity.

There are all kinds of actions so your bot can do different things like responding, opening pull requests, merging, and more. You can see all of the available actions in [Learning Lab's documentation](https://lab.github.com/docs/actions/).

## Step 9: Write the first Learning Lab action

You've got the response file, and now it's time to edit the `config` file with the proper action: respond. This will come after the event, or the trigger, as a "type". It will look like this:

```
  - title: Reference the template
    description: Edit the config file to reference your chosen template repository.
    event: pull_request.synchronize
    link: '{{ repoUrl }}/pull/2'
    actions:
    - type: respond
      with: 04_good-template.md
```

### :keyboard: Activity: Write the first Learning Lab action for a response into your course's configuration file

1. Edit the file in this pull request to add a respond type, referencing the file that you created for the response

<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
