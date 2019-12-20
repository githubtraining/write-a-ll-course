# Troubleshooting: Importing a course

If you're having trouble importing your course, here are a few tips for troubleshooting.

## I can't find the place to import

There are a few different ways to start a course:

- Through the Learning Lab course builder
- Manually

If you do this manually, follow the instructions in the ["Create the course on Learning Lab (manual option"](https://lab.github.com/docs/course-ownership-and-repositories#manual-repository-setup) paragraph.

This should lead you to a URL that looks like `https://lab.github.com/:owner/new`. _(Ex: https://lab.github.com/githubtraining/new)_

## My import fails and I don't know why

### Validate the YAML

Try to validate the YAML in the `config.yml` using a tool like [yamllint](http://www.yamllint.com/).

### Check response files

Check the responses referenced in the the `config.yml` file. Do they all exist? Are they in a directory called `responses`? Are there any typos?

### Get more detailed error messages

More detailed error messages are available for draft courses made from pull requests. To do this, the course must first be published. Create another branch with the most up-to-date version of your course. Edit the course version on the `master` branch to reduce the possibility for errors. (You can do this by matching [the boilerplate repository](https://github.com/githubtraining/write-a-ll-course-template/blob/master/config.yml).)

## Still stuck

If you're still stuck, visit us in the [Community Forum]({{ communityBoard }}) and we'll be happy to help!