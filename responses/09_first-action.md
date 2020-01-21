# Learning Lab Actions

Awesome! You're probably thinking - how is Learning Lab validating that I did the thing just now!? And you have a point. With text, it's tricky - so I checked to make sure you wrote more than 5 words, but I'm not checking to see if you wrote anything that makes sense. For this type of step, it would be difficult to provide great feedback on what you wrote.

Every comment that I make is an example of a real, human-proofed answer. Compare your answer and notice - is yours similar? Is it very different? What would you change?

### Action `type: respond`

Now that you've given me something to say, we need to figure out _how_ to say it to with Learning Lab. Now is the time to learn about Learning Lab's _actions_. Actions are reusable modules that each Learning Lab course has access to. They are each designed to do very specific things, and nothing more. This is to optimize for reusability and simplicity.

There are all kinds of actions so I can do different things like responding, opening pull requests, merging, and more. You can see all of the available actions in [Learning Lab's documentation](https://lab.github.com/docs/actions/).

## Step 9: Write the first Learning Lab action

You've got the response file, and now it's time to edit the `config` file with the proper action: respond. Because this is our first instruction, we will put it in the "before" step so the learner knows what we are waiting for them to do when they first enter the course. It will look like this:

```
    before:
    - type: respond
      with: 01_first-response.md
```

### :keyboard: Activity: Write the first Learning Lab action for a response into your course's configuration file

1. [Edit the `config.yml` file in this pull request]({{ url }}) on lines 17 and 18 to add a respond type, referencing the file that you created for the response.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
