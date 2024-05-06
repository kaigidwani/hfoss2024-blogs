---
layout: post
# If your post title is longer or more complicated
# than can be represented in the filename, uncomment the following line
# and specify a custom title
# title:  "Sample Blog Post"

# Uncomment only one of the below categories
categories: 
- Bug Fix
#- Contribution


# Enter your name below
author: Patrick Hurley
---

## What is MonoGame?
For my contribution, I decided to contribute to the MonoGame game engine.  MonoGame is a framework built off of Microsoft's now deprecated XNA Framework, and has been used to create many titles such as Celeste, Stardew Valley, and Barotrauma.  I decided to contribute to MonoGame because I've used it before, for a group game project I made in my freshman year, giving me some familiarity with how the engine works.  It also has a large amount of issue labels for easier categorizing and searching, with "Good First Issues" being the one I primarily used.

## Mini Comm Arch evaluation

MonoGame is a large and active repository comprised of a few dedicated multi-commit contributors and a large volume of drive by contributors.  The project's [code of conduct](https://github.com/MonoGame/MonoGame/blob/develop/CONTRIBUTING.md) is both easy to find and easy to comprehend, and the community as a whole seems very kind.  The project itself is growing in popularity, too, and is run as a Federation.

## Choosing an Issue
To find what issue I wanted to contribute to, I first checked the issues under the Good First Issues label, and settled on [Issue #4856](https://github.com/MonoGame/MonoGame/issues/4586) because it seemed like it wouldn't require an obscene amount of time to fix.  

![screenshot of Issue #4856](https://cdn.discordapp.com/attachments/1227366070466248706/1227366080524324874/image.png?ex=662824bc&is=6615afbc&hm=368e82f92effbcef78ee7de68183b765bc58c5bc2d9ef9df8e51c94aa143b361&)

Little did I know, it also required knowledge of 3d transformations and matrices, which were the one topic in calculus that I almost failed.  Not really understanding what the issue actually required me to document, I had the idea to look for other documentation-related issues, as I had already read every issue marked Good First Issues, and at the bottom of the conversation under Issue #4856 was a link to a project in the repository named [Improving the documentation and samples](https://github.com/MonoGame/MonoGame/projects/4#card-82244161).  Looking through the issues there, I found [Issue #4804](https://github.com/MonoGame/MonoGame/issues/4804), which is about writing documentation for a bug concerning how MonoGame's vsync settings interact with end user graphics driver hacks that can force different types of vsync.

![screenshot of Issue #4804](https://cdn.discordapp.com/attachments/1227366070466248706/1227378654237950114/image.png?ex=66283072&is=6615bb72&hm=b172ceaa83f0ea6885a9e84198632e422c1b7d653ea93944057d3e9c3b6ba3c0&)

## How was it 'fixed?'
As the issue I chose was related to writing documentation for an already discovered and diagnosed issue with graphics card drivers, I didn't have much to actually code myself.  I updated the \<remarks\> tag inside the comment for the SynchronizeWithVerticalRetrace method to specify that it could cause issues like multiple update calls per draw call, and that was it.  Then came the roadblock.  Or at least, the part I way over-analyzed, only to find out it was all unnecessary.

![screenshot of my commit](https://cdn.discordapp.com/attachments/1227366070466248706/1227381682848661524/image.png?ex=66283344&is=6615be44&hm=48bf8dcda68a89dcdcc9180aa2b7b1d0f60569da8a62c25b3520f3aeb8c50416&)

I had the changes in code pushed to my fork, but I wanted to know how to get those changes reflected in the project's documentation too, so I went there.  First I checked the [readme](https://github.com/MonoGame/docs.monogame.github.io/blob/main/README.md) of the documentation repo, which strangely didn't link to the repo's contributing page.  Because I didn't know the repo had one, I spent the next hour looking through the code in the repositiory trying to find out what I would need to change to add my part to the documentation, also checking the [framework that the documentation was built off of, docfx](https://dotnet.github.io/docfx/).  Still couldn't figure it out, until I noticed the [contributing.md](https://cdn.discordapp.com/attachments/1227366070466248706/1227383958086615171/image.png?ex=66283563&is=6615c063&hm=cbd3c134ff3d413017987031f663802efba795617fc17239834ff88d30113004&) file tucked away in the root folder of the repo, which mentions that the documentation is automatically "rebuilt when the code changes and is published nightly to the website."  So that was a fun way to spend an hour.  After that, I made a [pull request](https://github.com/MonoGame/MonoGame/pull/8269), and within a day recieved an approval from one of the project's maintainers and most active contributors, dellis1972.

![screenshot of my pull request and approval](https://cdn.discordapp.com/attachments/1227366070466248706/1227385141941243986/image.png?ex=6628367d&is=6615c17d&hm=5e9969124e407134456640de01c229d675f3da35baf2810ed4e9c020a7596e43&)

As of April 9th at 6pm, my change has not yet been merged into MonoGame's development branch, and judging by how old some other pull requests are, it's anybodies guess how long it may stay that way.





[jekyll-docs]: https://jekyllrb.com/docs/home
