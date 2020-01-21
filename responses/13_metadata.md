# Course metadata
  
Awesome work so far! Now, you've officially got your first step written. It's a good time to try this course out. Before we do, we need to pay some attention to the metadata in the config file, so that Learning Lab knows what to do with it.
  
The parts that we need now are the title, tagline, description, and the name of the learner's repo. Learning Lab also needs more detail around each step. The information is there in detail in comments in the config file.

Here are a few examples:

- [Introduction to GitHub](https://github.com/githubtraining/introduction-to-github/blob/master/config.yml)
```
title: Introduction to GitHub
tagline: Your sidekick for getting started on GitHub
description: If you are looking for a quick and fun introduction to GitHub, you've found it. This class will get you started using GitHub in less than an hour.
template:
  name: github-slideshow
  repo: caption-this-template
  description: 'A robot powered training repository :robot:'
```
- [Communicating Using Markdown](https://github.com/githubtraining/communicating-using-markdown/blob/master/config.yml)
```
title: "Communicating using Markdown"
tagline: "Your guide to mastering Markdown"
description: "This course will walk you through everything you need to start organizing ideas and collaborating using Markdown, a lightweight language for text formatting."
template:
  name: "markdown-portfolio"
  repo: "communicating-using-md-template"
```
- [This course - Writing a Learning Lab course](https://github.com/githubtraining/write-a-ll-course/blob/master/config.yml)
```
title: Write a Learning Lab course
tagline: Learn how to author your own Learning Lab course.
description: Use Learning Lab's strengths for fast feedback to author your own course.
template:
  name: lab-starter
  repo: write-a-ll-course-template
```

## Step 13: Create course metadata

**Important:** To ensure you can test this course, the template `name:` **must be different** than the name of this repository. The template name is what Learning Lab will name the repository when it is created on the learner's account. If the learner already has a repository with that name, it will fail --  so, make it unique.

### :keyboard: Activity: Add the course metadata like title and description to the configuration file

1. [Edit the config file]({{ url }}) (lines 1, 2, and 3) so the comments are gone, and your information is there.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
