---
layout: post
# If your post title is longer or more complicated
# than can be represented in the filename, uncomment the following line
# and specify a custom title
# title:  "Implement uninstaller.exe to wincuts"

# Uncomment only one of the below categories
categories: 
#- Bug Fix
- Contribution


# Enter your name below
author: Weijie Ye
---

# Why stick with Wincuts
I chose the same project for my Contribution as I did for my Bug Fix because I'm familiar with it. I worked on this project for my bug fix, and the project owner responded to me very quickly. There are several issues in this project that I also have the ability to complete, so I decided to work on Wincuts again for my contribution.
# What is Wincuts

[Project Website](https://lyubomirt.github.io/wincuts/pages/download.html)

[GitHub Page](https://github.com/LyubomirT/wincuts)

WinCuts is a Windows native (via Qt) tool for easily setting up and managing custom keyboard shortcuts. It's designed for simple usage and is aimed at anyone who wants to save time and increase productivity by using keyboard shortcuts.

# How it works
As of now, WinCuts lets you set up custom keyboard shortcuts for running shell/cmd commands that get launched whenever the shortcut is activated. It's useful if you need to launch specific commands frequently and want to save time by using a keyboard shortcut instead of typing the command every single time.
What's also cool is that none of the shortcuts will go deep enough in your system to cause any damage. They're all running in the context of the user and are limited to the user's permissions. And, of course, the shortcuts are only active within the app and hence won't interfere with any other shortcuts you might have set up (basically, you can't accidentally override a system shortcut).

# Why I picked Wincuts
I chose to contribute to WinCuts because it could improve my productivity when developing on Windows. Since I can fix several issues, I decided to help this project out.

# Resources
The project provided both [contribution guide](https://github.com/LyubomirT/wincuts/blob/main/CONTRIBUTING.md), [code of conduct](https://github.com/LyubomirT/wincuts/blob/main/CODE_OF_CONDUCT.md) and the license this project uses is BSD-3-Clause license.
Since this is a relatively new project, there are few participants, but the project's owner is very active; he can always respond to you within a day, from my experience.

One negative side of this project is the need for more documentation. This does make it difficult to understand the project at the beginning, but since this is a small project and the task I chose to do didn't interact too much with the main part of the software itself, this didn't cause too many problems when I was developing.

# The Issue
The issue I worked on in this project was Creating a help button inside the app. As the creator mentioned, many users won't go deep diving to try to find the repository's README; a simple Help button should work way better.
[issue](https://github.com/LyubomirT/wincuts/issues/2)

![wincutContributeIssue](https://github.com/wy8933/hfoss2024-blogs/assets/112401719/40334375-e7b3-4ed7-9392-dba93feeb7fa)


# Contribution process
First, I read the project's current repository's README, which contains all the information the user should know in order to use the app correctly.

Then, Start by adding the help button to the main program UI

![image](https://github.com/wy8933/hfoss2024-blogs/assets/112401719/cf87afd0-cb8a-4fb3-b0a8-a3f80da6ab8e)

After ensuring that the button is clickable and the user can navigate to the help window when clicking on it, I add information to the window.

![image](https://github.com/wy8933/hfoss2024-blogs/assets/112401719/623f8357-ca1c-4db9-9f24-85dd81581009)

Finally, I added the feature of clicking on the icon, which also shows the help button. Thus, the contribution has been made. 

![image](https://github.com/wy8933/hfoss2024-blogs/assets/112401719/916e9149-dab9-467f-9fe3-4f22e89d3ee6)


# Blocker
During the development, everything went smoothly since I had already contributed to this project before, so I understood how and what I should do. However, I didn't understand how to use the app in-depth, so I asked other people in the discussion, and the creator quickly answered my question and gave me several suggestions for improvement.
![image](https://github.com/wy8933/hfoss2024-blogs/assets/112401719/6b3c4560-6ac2-4aa2-8a94-007f5abb0281)

# Pull Request
As of the writing of this blog post, the PR opened was accepted 
[Link to pull request](https://github.com/LyubomirT/wincuts/pull/13)

# Conclusion
Overall, I had a good experience working on this issue and project. While the specific problem I chose to work on was pretty simple, this was an excellent experience, and the author put my name on the newest release with credit for my contribution.
![image](https://github.com/wy8933/hfoss2024-blogs/assets/112401719/0858ad0e-e130-44fe-83b3-5baf4dd0b2b2)


