---
title: "First Open Source Contribution"
layout: post
date: 2023-11-14 15:59
image: /assets/images/markdown.jpg
headerImage: false
tag:
- markdown
- elements
- fork
- clone
- branch
- push
- pull-request
star: true
category: blog
author: johndoe
description: Markdown summary with different options
---

## How to Make Your First Open Source Code Contribution
<!-- 
This note **demonstrates** some of what [Markdown][1] is *capable of doing*.

And that's how to do it. -->
![Markdowm Image](https://www.freecodecamp.org/news/content/images/size/w2000/2023/07/IMG_6828-1.jpeg)
To begin, you are going to be using [First Contributions](https://github.com/firstcontributions/first-contributions). This is a popular project that helps beginners make their first open-source contribution. You'll also use GitHub's Codespaces, your local development environment on the cloud, to enable a smooth contribution process.

To get started, you will need to create a GitHub account if you don't already have one. Follow the signup process [here](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F%3Cuser-name%3E%2F%3Crepo-name%3E&source=header-repo&source_repo=firstcontributions%2Ffirst-contributions). All done? Let's get started.

<!-- {% highlight html %}
This note **demonstrates** some of what [Markdown][some/link] is *capable of doing*.
{% endhighlight %} -->

---

## How to Make Your First Open Source Contribution

There are six levels of headings. They correspond with the six levels of HTML headings. You've probably noticed them already in the page. Each level down uses one more hash character. But we are using just 4 of them.

### Step One: Fork the Repository

To fork a repository means to make a copy of the repository in your GitHub account. This enables you to make changes without disrupting the main project.


* First, click the "Fork" button at the top right corner of the repository.

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/fork.PNG)

* Then click on the "Create Fork" button at the bottom of the page, similar to the screenshot below.

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/createe.png)

* If it's successful, firstcontributions/first-contributions will flick over to your account name / first-contributions.

### Step Two: Clone the Repository

Codespaces automatically sets up a development environment for you with the repository already cloned. There's no need to through the manual setup with your local terminal.

* Click on the green "Code" button

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/code.PNG)

* Select "Codespaces" from the dropdown menu, then click on the "Create codespace on main" button.

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/codespacess.PNG)


### Step Three: Create a Branch

When using Codespaces there’s no need to change directories because the repository is already available in the current directory.

To create a new branch, you will need to type this command on your terminal:

{% highlight raw %}
git switch -c your-new-branch-name 
{% endhighlight %}

That is the git switch -c command along with what you want to name your branch.

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/A.PNG)

### Step Four: Make Your Changes

The only change you'll make for this tutorial is to add your name and a link to your GitHub account to the CONTRIBUTORS.MD file. This marks you as a contributor

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/D.PNG)

### Step Five: Commit and Push

Now you'll need to stage your changes by adding the changes that are ready to be committed. You can do this with the following command:

{% highlight raw %}
git add . or git add Contributors.md  
{% endhighlight %}

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/D.PNG)

Then commit your changes using the command below:

{% highlight raw %}
git commit -m "Add [your name] to the Contributor List"  
{% endhighlight %}

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/C.PNG)

Finally, push your changes to the repository like this:

{% highlight raw %}
git push -u origin your-branch-name 
{% endhighlight %}

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/E-1.PNG)

Once you see something similar to the screenshot below, you are on the right track.

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/F.PNG)


### Step Six: Create a Pull Request

A pull request alerts the repository's maintainers to the changes you've made. It allows them to review these changes before merging them into the main repository.

To create a PR, follow these steps:

* Switch to your branch once you refresh your repository. 

* Click on the “Compare and pull request button” that appears.

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/G.PNG)

* Write a description of what you did then click on the "Create pull request" button. 

![Markdown Image](https://www.freecodecamp.org/news/content/images/2023/07/H.PNG)

Once you finish, the Frist contributions bot or the maintainers will merge your changes if they're good to go

### Conclusion

Congratulations! You have made your first contribution to open source. This is an exciting milestone that marks the beginning of your journey as a contributor.

But don't stop there – there are hundreds of open-source projects on GitHub that need your help. Explore new projects and keep contributing.