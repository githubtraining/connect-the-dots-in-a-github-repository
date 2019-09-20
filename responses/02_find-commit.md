# Finding commits

An important part of version control is the ability to look into the past. By using `git blame`, and finding the story behind a commit, we're able to do more than _blame_ people for code. We're able to see the story around why a commit was made - what is the associated pull request? Who approved the pull request? What tests were run on that commit before it was merged?

The obvious reason to find things in history is to know about history. With issues and pull requests, we see a more complete story about history - not just the bare minimum.

### What's `git blame`?

Git Blame is a Git functionality that shows what revision and author last modified each line of a file. Information like who made a commit, when, and even why can be found this way. If you aren't sure who introduced certain changes to a file, you can use `git blame` to find out. While `git blame` sounds rather accusatory, this can be used to understand the context around decisions.

### What's a SHA?

A SHA is a reference to a specific object. In this case, it's a reference to a commit. On GitHub, you can look at a specific commit to see the changes introduced, by whom, and if they were a part of a pull request.

## Step 3: Find the commit

### :keyboard: Activity: Find and reference the navigation commit

1. Find the commit where the `docs/_sidebar.md` file was added
2. Copy some part of the SHA (at least the first 6 characters)
3. Comment (at least the first 6 characters of) the SHA in this issue
