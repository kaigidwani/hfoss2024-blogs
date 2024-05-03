---
layout: post
# If your post title is longer or more complicated
# than can be represented in the filename, uncomment the following line
# and specify a custom title
# title:  "CHAOSS Slack Bot Contribution" 

# Uncomment only one of the below categories
categories: 
#- Bug Fix
- Contribution


# Enter your name below
author: Isha Errande 
---

For my contribution, I chose to contribute to the CHAOSS slack bot. The slack bot is built using bolt for javascript. The current main goal for this particular project is to make it easier for beginners to contribute. 
I mainly did fixes to the main SETUP.md file and contributed ideas for the wiki. 

## Introduction to Issue 
Back when I was trying to make a contribution for my bug fix, I contacted CHAOSS both on slack and through their github to attempt to find an issue. I originally commented under issue [number 98](https://github.com/chaoss/chaoss-slack-bot/issues/98). I got a reply after after I completed my bug fix for a seperate project. 

![image](https://github.com/ise8933/hfoss2024-blogs/assets/90360951/2913d295-d791-4eed-9048-551cf70da592)

The new issue consisted of adding a missing step within the setup doc. This is [issue 101](https://github.com/chaoss/chaoss-slack-bot/issues/101)
![image](https://github.com/ise8933/hfoss2024-blogs/assets/90360951/f950660a-2ff9-44af-9d85-75247e00b557)


## Why not something else, like WordPress?
HFOSS is a class designed to help teach some of the basics behind open source. By using git and GitHub to submit the blog posts, there are more opportunities to practice using the tools that are used by real-world projects. Additionally, the WordPress sites from previous classes are no longer around and are hard to point to as examples that are particularly positive or negative.

## How do I use it?
This repository may look like a mess of many, many files, but realistically the only files you will likely care about as an HFOSS student are in the `_posts` folder. This is where you will upload your blog posts. The basic process goes something like this:

1. Log into your GitHub account
2. Create a fork of this repository and clone it to your computer if that's how you prefer to work (feel free to try a few different ways)
3. Create a new branch on your fork starting from the `main` branch
4. Find the `_posts` folder and create a copy of this sample post, giving it a new, dated filename (Jekyll requires blog post files to be named according to the following format `YEAR-MONTH-DAY-title`) and changing the contents accordingly (ideally making commits and pushing to your new branch as you go)
5. [Optional] You can also configure github pages (through the settings tab of your forked repository) to host a website site based on your new branch, so you can preview your changes and make sure your post looks the way you want. There are also ways to assemble the website on your computer if you prefer a more hands-on process (Ask in class or come to office hours if you want to learn more about this!) 
6. When you are ready to submit, create a "pull request" back to the original repository. This will take the contents of your new branch and submit it as a proposed change to the main class website. Once approved, your blog post will be added to the main class web page.
7. [Recommended] Whenever the main class webpage updates, it may be helpful to also update the main branch of your fork (github provides a handy "sync" button) so that you can stay up to date



## More Markdown features
In addition to the formatting used so far in this document, Markdown offers several other things that may be useful to blog posts. 

### Images

![a meme depicting a cartoon person screaming "OPEN SOURCE"](https://ankitrokdeonsns.github.io/assets/img/open_source.jpeg)


[Here](https://www.markdownguide.org/basic-syntax/#images-1) is a link to more documentation on markdown images.

### Tables

| Item         | Price    | # In stock |
| ------------ | -------- | ---------- |
| Juicy Apples | 1.99     | *7*        |
| Bananas      | **1.89** | 5234       |

[Here](https://www.markdownguide.org/extended-syntax/#tables) is a link to more documentation on markdown tables.

## More Jekyll Features
Jekyll can also provide some formatting and other useful features. Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. Here are some notable examples:


### Code snippets

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}


[jekyll-docs]: https://jekyllrb.com/docs/home

