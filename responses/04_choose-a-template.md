# Choosing a Template

One of the things that makes Learning Lab special is the ability to learn a skill _in context_. As you think about what you want to teach, it's critical to think about the context that you want to teach your topic in. 

Most courses make use of a [:book: template repository](https://lab.github.com/docs/course-ownership-and-repositories#the-repositories). Learning Lab clones the template repository from your account and then uses it to create a new repository on the learners account. Template repositories contain starter code and resources to help learners find their way.

> The template repository you designate will need to be owned by _the same account as this course repository_.

When creating or choosing a template repository for your course, consider two main points.

### Creating relevant content

First, how will this content help teach the concept? For example, if a course is teaching HTML, the success of the finished product should feature HTML.

If you're teaching JavaScript, an app makes sense. If you're teaching Markdown, maybe you don't need a project at all! With CSS, you could use a project relating to design.

Think of a project that is "real" and practical with the skill you're teaching. Don't introduce too many additional, and possibly confusing, concepts.

### Finished product

Second, is the finished product useful? At the end of the course, the finished repository should serve a purpose aside from the lessons. A working game, a portfolio or resume, or a collection of template documents are a few examples.

## Step 4: Reference the template

Select a template repository - or use ours - based on the points listed above.

### :keyboard: Activity: Edit the config file to reference your chosen template repository

1. Choose a repository to be a template.
    - It's important that {{ owner }}, the owner of _this_ repository, is also the owner of the template repository.
    - The template repository doesn't have to be complete at this point, but it should have at least one commit. If you don't know where to begin, create a new repository with a README on your account.
    - To ensure you can test this course, the template `name:` **must be different** than the name of this repository. The template name is what Learning Lab will name the repository when it is created on the learner's account. If the learner already has a repository with that name, it will fail --  so, make it unique.
2. [Edit the `config.yml` file in this branch]({{ url }}) to replace the commented template `name` and `repo`.
    - **Important!** Make sure the `name:` field is _different_ than this repository! Otherwise, you won't be able to take your own course.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
