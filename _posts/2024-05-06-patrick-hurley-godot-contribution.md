---
layout: post

title:  "Godot Documentation: Resource Loading"

# Uncomment only one of the below categories
categories: 
#- Bug Fix
- Contribution


# Enter your name below
author: Patrick Hurley
---

## What is Godot?
Godot is an open-source game development engine that is maintained by a small group of people who oversee and approve all issues and pull requests. Godot uses its own unique language called GDScript, which is similar to Python, but it also supports c# usage with the .net version. It has come more into the spotlight recently with Unity's monetization changes this past fall.

![godot logo](../assets/2024-05-06-patrick-hurley-godot-contribution/godot-logo.webp)

## Why pick Godot?
Initially, Unity's pricing model fiasco put Godot on my radar as a cool game engine.  More recently, a group in one of my game dev courses made a platformer using the engine that I helped playest, which reminded me of the project when it came time to contribute.  I wasn't sure if I wanted to contribute to MonoGame again for this project or not, but I chose to contribute to Godot after taking a look at its very, very detailed wiki, which leads me into the next section...

### Is Godot a good project to contribute to?
Yes.  The project has multiple lines of communication available to potential contributors and users, with extensive documentation on methods in Godot, building Godot from source, contributing to the project, and even on git functions like rebasing (which they ask that you use so small contributions only comprise a single commit).  

### Godot resources I used to help me help them
For the work itself, I referenced the [resource loader documentation](https://docs.godotengine.org/en/latest/classes/class_resourceloader.html) to learn a bit more about the code I would be writing documentation on, and referenced the C++ [header file](https://github.com/godotengine/godot/blob/7cdad333114e6765351ed0facb48db228ef29b7b/core/io/resource_loader.h#L74) and [source file](https://github.com/godotengine/godot/blob/7cdad333114e6765351ed0facb48db228ef29b7b/core/io/resource_loader.cpp#L147) to see firsthand how the method worked.  I also referenced the [content guidelines](https://docs.godotengine.org/en/latest/contributing/documentation/content_guidelines.html) and [writing guidelines](https://docs.godotengine.org/en/latest/contributing/documentation/docs_writing_guidelines.html) to ensure my contribution was stylistically consistent with the rest of the project and easy to comprehend.

When it came time to create my pull request, I read the [pull request review process](https://docs.godotengine.org/en/latest/contributing/workflow/pr_review_guidelines.html), which told me the format that Godot preferes for contributions.  Linked from there, the [pull request workflow](https://docs.godotengine.org/en/latest/contributing/workflow/pr_workflow.html#doc-pr-workflow) page gave step-by-step instructions on how to format my contribution so all of my commits could be "rewritten" into just one, so the main projects commit history could be easily readable.

## The Issue
### How I decided on my issue
For my contribution, I wanted to contribute to Godot's documentation, as I'm one of those strange people who actually enjoys writing documentation and combing through code trying to puzzle out its purpose.  That, and I'm a bit rusty on my coding skills and didn't want to make a sub-par contribution to the project, so I stuck to something I'm very confident in.

I started looking for an issue in the [godot-docs](https://github.com/godotengine/godot-docs) repo, as thats the one I figured most documentation issues would be in, and found an issue posted just three days before I began my search.  I knew I wanted to do this one just as a glance, as I could tell from the description of the issue that this was one of those "'minor' problems that break your code for four hours while you try to diagnose them," and having just finished another 10-week game mod project for IGME 424, problems like those hurt my soul.



### Similarities and differences from my bug fix

### My initial plan for contributing

### Expectations, meet reality

### Conclusion

