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

![screenshot of a view of a commit on GitHub, highlighting the link to the pull request](https://github.com/githubtraining/working-in-large-repositories/blob/master/responses/images/pr-link.png?raw=true)

## Step 4: Give more context

In the story above, you might want to `@mention` the authors involved in the article. You may want to find them in person, or set up another way to collaborate. In this case, we want to bring the information that you found through the commit to the greater conversation.

### :keyboard: Activity: Reference the related pull request in this issue

1. In the tab where you found the commit SHA in the last step, click the link to the related pull request
2. Copy a reference (like a link) to this pull request
3. Comment with a link to the "Add Navigation" pull request in this issue

