---
title: "Adding  locally hosted code to Github (Windows)"
layout: post
date: 2023-11-14 16:02
image: ../docs/assets/images/markdown.jpg
headerImage: false
tag:
- push
- commit
- bash

star: true
category: blog
author: johndoe
description: Markdown summary with different options
---

## Adding locally hosted code to GitHub

If your code is stored locally on your computer and is tracked by Git or not tracked by any version control system (VCS), you can import the code to GitHub using GitHub CLI or Git commands.

### About adding existing source code to GitHub
If you have source code stored locally on your computer that is tracked by Git or not tracked by any version control system (VCS), you can add the code to GitHub by typing commands in a terminal. You can do this by typing Git commands directly, or by using GitHub CLI.

### Initializing a Git repository
If your locally-hosted code isn't tracked by any VCS, the first step is to initialize a Git repository. If your project is already tracked by Git, skip to [Importing a Git repository with the command line.](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github#importing-a-git-repository-with-the-command-line)


1. Open Git Bash.
2. Navigate to the root directory of your project.
3. Initialize the local directory as a Git repository. By default, the initial branch is called main.

{% highlight raw %}
git init -b main
{% endhighlight %}

4. Add the files in your new local repository. This stages them for the first commit.

{% highlight raw %}
git add .
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
{% endhighlight %}

5.Commit the files that you've staged in your local repository.

{% highlight raw %}
git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
{% endhighlight %}

### Adding a local repository to GitHub using Git

1. Create a new repository on GitHub.com. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub. For more information, see ["Creating a new repository."](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

2. At the top of your repository on GitHub.com's Quick Setup page, click  to copy the remote repository URL.

![Markdown Image](https://docs.github.com/assets/cb-48149/mw-1440/images/help/repository/copy-remote-repository-url-quick-setup.webp)

3. Open Git Bash.

4. Change the current working directory to your local project.
5. To add the URL for the remote repository where your local repository will be pushed, run the following command. Replace REMOTE-URL with the repository's full URL on GitHub.

{% highlight raw %}
git remote add origin REMOTE-URL
{% endhighlight %}
6. To verify that you set the remote URL correctly, run the following command.
{% highlight raw %}
git remote -v
{% endhighlight %}
7. To push the changes in your local repository to GitHub.com, run the following command.

{% highlight raw %}
git push origin main
{% endhighlight %}
