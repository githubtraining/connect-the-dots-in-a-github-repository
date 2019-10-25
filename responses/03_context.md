# Context

As we've already seen, conversations in issues and pull requests can reference other work.

But the amount of context goes much further than crosslinks - Remember, Git is version control! For example, the commit that you found in the last step is connected with much more information: 

- Who made the commit
- What other changes were included
- When the commit was made
- Which pull request the commit was a part of

The pull request is important because it goes beyond knowing when a commit happened - you can know _why_ a commit happened. Finding history is not about _blaming_ anyone, but about seeing the bigger picture. Why were decisions made? Who was involved? What were the build outputs and test results for each commit? Who requested changes, and who approved them?

### A story about finding experts

Imagine you find an internal white-paper on a really exciting topic. You're looking for experts to help you research this topic for an upcoming project. When you find this article, you're ecstatic! But, there's no author referenced in the plain text.

You can see that it's written in markdown, and it's versioned in GitHub. It's already a part of the `master` branch, but you want to know who was involved in creating this. You use `git blame` to see the author(s), and you can find the pull request associated with that branch. Now, you can see who all of the authors were, who the reviewers were, and if there are any other issues or conversations related to this topic.

Just like that, you've found the people at your company who can help move your project forward. :tada:

### Finding a pull request from a commit

When you're looking at a commit on GitHub, you can see a lot of information. From this view, you can also find a link to the pull request in which the commit was created. We'll use this in the next step.

![screenshot of a view of a commit on GitHub, highlighting the link to the pull request](https://user-images.githubusercontent.com/16547949/67341250-3edbb480-f4fd-11e9-805a-6bce5a8ba2d1.png)

## Step 4: Give more context

To help others find relevant context, we want to collate the information that you found in the prior steps.

![a screenshot of this issue with the projects section highlighted on the right, and a second screenshot of v1.0.0 project](https://user-images.githubusercontent.com/16547949/67590688-b0984600-f729-11e9-8d46-cc243d666331.png)

One way we can do this, is by using [GitHub Projects](https://help.github.com/en/github/managing-your-work-on-github/about-project-boards). You'll notice that this issue is part of [Project v1.0.0]({{ repoUrl }}/projects/1), which tells us that the sidebar is part of the work related to our version 1.0.0 release. Let's add the related pull request to the same project so that the two artifacts can be tracked in tandem.

### :keyboard: Activity: Use a project to track related efforts

1. Go back to {{ commitId }}.
1. Click the link to the related pull request.
1. In the pull request, click on **Projects** on the right side, and choose the `v1.0.0` project from the list.
1. When the PR is added to the project, you'll see it's _Awaiting triage_, let's triage it! Click on the project drop down, and place it into the **Done** column.

I'll respond in this issue when you've added the pull request to the In Progress column of the v1.0.0 project.