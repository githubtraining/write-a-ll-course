Uh oh! I see that this branch now has a merge conflict. A **Merge conflict** occurs when changes are made to the same part of the same file on two different branches. You usually find out about conflicts in a pull request. 

If you've solved merge conflicts before, you know what to do: go ahead and resolve it now.

If this is your first merge conflict, that's OK too. Here are instructions for resolving a merge conflict:

1. At the bottom of the page in the "This branch has conflicts that must be resolved" section of the Pull Request, click the **Resolve conflicts** button.
2. Look for the highlighted sections that begins with  `<<<<<<<  template` and ends with `>>>>>>> main`. These markers are added by Git to show you the content that is in conflict.
3. Choose the version that you'd like to keep - do you want to keep the content between `<<<<<<<  template` and `======`, or `======` and `>>>>>>> main`? 
4. Delete the content that you do not want to keep.
5. Next, remove the merge conflict markers by deleting the following lines:

       <<<<<<< template
       =======
        >>>>>>> main

6. With the merge conflict markers removed, click **Mark as resolved**.
7. Finally, click **Commit merge**.