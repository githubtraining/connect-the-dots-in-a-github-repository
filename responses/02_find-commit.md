# Finding commits

An important part of version control is the ability to look into the past. By using `git blame`, and finding the story behind a commit, we're able to do more than _blame_ people for code. We're able to see the story around why a commit was made - what is the associated pull request? Who approved the pull request? What tests were run on that commit before it was merged?

The obvious reason to find things in history is to know about history. With issues and pull requests, we see a more complete story about history - not just the bare minimum.

### What's `git blame`?

`git blame` is a Git functionality that shows what revision and author last modified each line of a file. Information like who made a commit, when, and even why can be found this way. If you aren't sure who introduced certain changes to a file, you can use `git blame` to find out. While `git blame` sounds rather accusatory, this can be used to understand the context around decisions.

### What's a SHA?

A SHA is a reference to a specific object. In this case, it's a reference to a commit. On GitHub, you can look at a specific commit to see the changes introduced, by whom, and if they were a part of a pull request.

## Step 3: Find the commit

### :keyboard: Activity: Find and reference the navigation commit

1. Navigate to the [Code tab of this repository]({{ repoUrl }})
   - _Tip: start this process in a new tab, since you will need it later_
2. Click `docs` to navigate into the `/docs` directory
3. Click `_sidebar.md` to view the file
4. On the top right side of the file, click **Blame** to see the details of the most recent revision
5. Click the commit message, `add sidebar to documentation` to see the commit details
6. Copy some part of the SHA (at least the first 6 characters of the 40 character hexadecimal string listed after `commit`)
7. Comment (at least the first 6 characters of) the SHA in **this issue**
