# 3 phases of a step

Have you ever thought about what teaching _is_? What are the behaviors that a good teacher has to make it easy to learn? Maybe you have - and maybe you haven't.

Let's break down teaching into three steps: 
- telling the learner what to do
- watching them to see if they do it or not
- giving them specific feedback about what they did or didn't do right. 

Repeat! That may sound simple, but it's the basis of fast feedback that is _learning_. :rainbow:

Just like we broke down your teaching goal into smaller steps, let's break down _teaching_ in the same way. Let's focus on the smallest possible unit of behavior we can identify.

For starters, let's choose writing unordered lists in Markdown. That's what we want the user to know how to do. Let's apply those three phases.

### Phase 1: Tell the learner what to do

What does the learner need to be able to exhibit the behavior that we want? Well, they'd need to know about Markdown, and it'd be nice if they had a computer with a keyboard, and a place to type the text. Let's assume those contextual things are taken care of. The main information that a learner would need would be, what is an unordered list? How is that written in Markdown? Then, we'd ask the user to do that.

### Phase 2: The learner does it and we observe

There's an important part of this step. It's not just the learner doing it, but it's how we are going to watch and observe if they did it correctly or not. In Learning Lab, this is usually an issue comment or a commit changing a file. We give them the space to try it out, and we watch via webhooks. We use gates to "check" if they did what we asked them to.

### Phase 3: Give the learner feedback

Based on the observation in the second phase, we can give them the feedback they need. We either confirm that they learned it, or let them know that they _didn't_ do it right, and they should try again. It's important to give the most specific feedback as possible. This is like unit tests - if they're vague, they're not helpful. The more personalized and exact the feedback can be, the better the learner will understand what they did right and/or wrong.

### How learning happens

This is how _all_ learning happens, through feedback, whether it's from a teacher in a classroom, a bot like me, or a stovetop that gives you the feedback "if you touch me, it HURTS!". Faster and more exact feedback is always a better teacher.

This is the process that we are going to use for each of the learning objectives you've written.

## Step 7: Choose the example that shows the three phases

Before we start writing some for this course, let's practice identifying this three phase process. There are four examples below - some of which are examples of this three phase process, and some of which _aren't_. For each example, there is a label. For each example that _is_ a good example of the three phases, add the corresponding issue label to this pull request. Once all of them match what I expect, I'll give you the next instructions.

If you get stuck, add the issue label "help" and I'll give you some more detail. (include instructions for how to add labels)

### :keyboard: Activity: Apply a label that corresponds to the example showing the three phases of a step

1. Read the following examples, and their corresponding "labels". (Click the triangle next to each title to drop down the full text.)
2. When an example correctly includes all three phases, add the corresponding label to this issue. (You can include multiple labels!)
    - _Not sure how to add a label? On the right side of this issue, you'll see a section titled **Labels**. Click the word **Labels** to bring up a menu. Click a label title to toggle adding or removing it from an issue or pull request._
    - If you get stuck, apply the `help` label.

<details>
 <summary>1: Committing a header</summary>
 <br>
 
 - **Phase 1**: We open a pull request for the learner that is adding a blank markdown file. We tell them what headers are, and show them examples of how to write them using markdown syntax. We ask them to commit a change to the file in the pull request adding a header.
 - **Phase 2**: The learner commits and changes the file.
 - **Phase 3**: We accept the learner's commit and move on to the next step.

</details>

#### 



<details>
 <summary>2: Closing an issue</summary>
 <br>
 
 - **Phase 1**: We comment in an existing issue and ask the user to close that issue. We explain what closing an issue means, that issues can be reopened, and give examples of when it's appropriate to close an issue.
 - **Phase 2**: We use the webhook event specifically for closing issues. The learner closes an issue. We use a gate to validate that the correct issue is closed. Using this gate, we determine that the learner closed the wrong issue.
 - **Phase 3**: We reopen the issue that was closed but should have stayed open, and we comment telling the user that they closed the wrong issue. We link to the correct issue.

</details>

<details>
 <summary>3: Fixing a bug
</summary>
 <br>

 - **Phase 1**: We open a pull request for the learner in a repository with tests configured. The learner has already demonstrated the skills needed to understand the tests and the codebase. The pull request introduces a bug and has a failing test. We ask the learner to change the files in that pull request to fix the bug and make the tests pass.
 - **Phase 2**: The learner commits changes. We check using gates that the tests are passing, and that the tests haven't been removed. We see that the tests are passing.
 - **Phase 3**: We merge the pull request for the user and create the next task. We comment in the pull request congratulating them, and link them to their next instructions.

</details>

<details>
 <summary>4: Writing a function</summary>
 <br>

 - **Phase 1**: We are teaching about writing functions, and we give the learner several examples in an issue comment. We ask the learner to write a function.
 - **Phase 2**: We assume the learner will create a branch, make a commit, and open a pull request. Then, we will use a gate to check their function. Because we ask the learner to do this in an issue, the learner is unsure of where to do this. They write a function as a comment in the issue.
 - **Phase 3**: Since we are listening for a commit, and the gate is set to check after that event, there is no feedback triggered when the user comments on the issue.

</details>

