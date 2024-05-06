---
layout: post
# If your post title is longer or more complicated
# than can be represented in the filename, uncomment the following line
# and specify a custom title
# title:  "Loading huge JSON datasets for Scene Links"

# Uncomment only one of the below categories
categories: 
#- Bug Fix
- Contribution


# Enter your name below
author: Erin Ford
---

For my contribution, I decided to continue to work on the Scene Links project that I mentioned in my Bug Fix blog post. There's a lot of things somewhat broken and unimplemented in it, so I decided I wanted to reimplement two of the major things that were bugging me about it: the JSON loading and graph legend.


## The Issue
Before I added my fix for the JSON, the person who invited me onto this project does not know very much about web development. They are working with a very large and somewhat disorganized dataset, and need to be able to easily load and modify that dataset without messing with the overall code architecture too much. The JSON dataset was literally copy-pasted into the main graph handler file, canvasGraph.js. This was because they didn't know about CORS and kept getting errors when trying to load JSON files based on tutorials online. This is a terrible way of doing things since it makes the dataset more annoying to modify and the code a pain to access. On top of this, there wasn't an actual legend for the fully rendered web. So, along with some miscellaneous reformatting of all the JSON so I didn't completely lose it, I set out to make my contribution.

## The Contribution
I added a little fixed floating legend in the bottom right hand corner of the graph. That was relatively simple to do, as I just needed to grab the color IDs of the different labels on the graph and add them to a list. Unfortunately, I had problems with getting the correct color matching with my text, but it's fine for now. As for the JSON, I had to delete all of the muck that was already in canvasGraph so that I could create a more elegant solution. I just did a fetch request for the specific graph JSON that needs to be loaded (planning to add a drop down menu to change which graph is applied later!) and set that to the same variable from before so it wouldn't break anything. There is, however, a bug where sometimes the JSON will not load and throws an exeption. This will require me to restructure the rest of the graph initialization code to force itself to wait for the response using async/await, which I am currently in the process of fixing.


Also, this isn't entirely related, but both creating this blog post PR and the contribution I am discussing are the first times I've properly done everything (except writing the pr on the github website) all in the CLI. I just got a new laptop and started running Fedora Workstation as my daily driver, so getting everything running and familiarizing myself with the Linux workflow has been a project in its own right.

Commit Links:

- [OG Pull Request](https://github.com/Scene-Links/Scene-Links/pull/4)
- [Small fix to PR](https://github.com/Scene-Links/Scene-Links/pull/6)