Great! When you commented, you triggered something called a webhook that I heard, and now I'm here! You may be wondering if I checked to see if  what you wrote was a _real_ topic. We'll talk about that kind of logic later - both how to use it, and when to use it. (Spoiler - for this step, I didn't check! I am pretty smart, but not smart enough to tell if you typed a good idea or not.)

### Breaking goals into smaller steps

Now that you know what you want to teach, the next thing to do is break it down into steps. This can be tricky - put on a teacher hat and an engineer hat at the same time.

To break down the thing you want to teach, think about the observable behaviors. They should show that the user is doing it right. If you were watching this person, how would you know they've mastered the thing? Some examples are:

- Close an issue
- Write a functional SQL query
- Merge a pull request
- Change code so a particular test passes

### How many goals?

The right number of "goals" may be different for different courses. But, our courses usually have between 7 and 20. For example, in the Communicating Using Markdown course, the steps (or goals) are:

- Create a task list
- Turn on GitHub Pages
- Add headers
- Merge your headers
- Add an image
- Add a profile link
- Merge your image and profile link
- Add a list
- Use emphasis
- Merge lists and emphasis

### What NOT to do

It is _not_ a good idea to have huge or ambiguous steps.

Put yourself in the shoes of a beginner. If you're asked to do something too big that you don't understand, it can be frustrating. Asking the learner to do something poorly defined creates confusion and misunderstandings. This can make the learner give up!

> Imagine you're taking a course on SQL as a beginner. If one of the steps is to write a full query, you might not know where to start. You may try your best, but still be confused about what isn't working. Or, if you can get it right from copying and pasting, you wouldn't understand it well enough to do it on your own. Stick to smaller steps, and include prerequisites at the beginning of the course.

## Step 2: Break your course into smaller steps

In the file in this pull request, write the steps as observable behaviors. It's OK if there are a lot. It's better to break it down into small steps. Then, you may realize the scope of the course is wrong. That is better than having huge or unmanageable steps.

> What's `#` in YAML? Any lines starting with `#` in the `config.yml` file are _comments_. We will use these for planning and documentation.

### :keyboard: Activity: Break down what you'd like to teach into smaller learning objectives

1. [Edit the `config.yml` document]({{ url }}). Break down the larger goal into smaller steps and add them to the commented descriptions on lines 26, 35, 40, 47, and 54.
2. In each step, notice the fields for `title` and `description`. These will be shown to the learner on Learning Lab. Write the titles and descriptions of each of your steps.
    - _You only need to worry about the title and description now. We'll fill in the rest later!_
3. Commit your changes.
4. Navigate _back_ to this pull request.

<hr>
<h3 align="center">I'll respond in this pull request when I detect a commit on this branch.</h3>
