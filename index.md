---
title: Home
layout: home
nav_order: 1
permalink: /
---

# Git & GitHub Documentation Wiki
## Group 01 - Riley, Alex, Nova, Traigen, and Gus!

Welcome to our Git & GitHub documentation wiki!

This website serves as a quick-reference guide for game development programmers and artists looking to learn about Git, GitHub, and version control.

Our documentation covers Git fundamentals, common commands, branching, merging, and collaborative workflows, with practical examples relevant to game development.

## The Role of Version Control in Software Development

Version control, also known as revision control or source control, is the management of changes to documents such as computer programs.

In software development, it helps developers manage different versions of a project, collaborate with others, recover older versions, and safely test new features.

Unlike simply using `Ctrl + Z`, version control allows developers to undo changes made weeks ago, restore older versions of files, and manage changes made by other team members.

### Pros of Version Control

Version control provides developers with much more than just the ability to undo changes.

- Tracks changes made to a project over time.
- Makes it easy to restore older versions of files.
- Allows developers to work on new features while fixing bugs in older versions.
- Helps multiple developers collaborate without overwriting each other's work.
- Allows distributed teams to work together on projects from anywhere in the world.
- Makes testing new features safer.
- Helps identify when bugs were introduced.

Version control is useful for both individual developers and teams, providing a safety net throughout the development process.

### Types of Version Control

#### Local Version Control

Stores different versions of files on one computer. It is simple, but not ideal for team projects.

#### Centralized Version Control

Stores the main project on a central server. Developers connect to the server to access and update files.

Examples include:

- Perforce Helix Core
- Subversion (SVN)
- CVS

#### Distributed Version Control

Each developer has a full copy of the project and its history. Developers can work independently and synchronize their changes.

Examples include:

- Git
- Mercurial

### Version Control in Game Development

Version control is especially useful in game development, where programmers and artists often work on the same project.

For example, in a Unity project:

- Programmers can track changes to scripts and game mechanics.
- Artists can manage changes to textures, models, and other assets.
- Team members can work on different features without directly overwriting each other's work.
- Developers can restore earlier versions if a new feature introduces problems.

Different version control systems are commonly used in game development:

- **Git:** A free, open-source distributed version control system commonly used in software development and game projects.
- **Unity Version Control:** A version control solution designed for game development teams, including programmers and artists.
- **Perforce Helix Core:** A centralized version control system widely used by larger game development studios.
- **Subversion (SVN):** A centralized version control system that can be used by smaller development teams.

## What Is Git?

Git is a free, open-source distributed version control system used to track and manage changes to files throughout a project's development.

Git allows developers to save different versions of their projects, restore previous changes, and collaborate with others.

When combined with hosting platforms like GitHub or GitLab, Git also allows developers to share their work with teams remotely.

### How Does Git Work?

Git tracks changes through repositories, which contain a project's files and their version history.

When developers make changes, they can create a **commit**, which acts as a save point for the project.

Each commit records a snapshot of the project at that point in time, allowing developers to review previous versions and recover earlier work.

Git also supports **branches**, allowing developers to work on new features or bug fixes independently before merging their changes into the main project.

Because Git is distributed, developers can work offline and synchronize their changes with remote repositories when connected.

### Pros of Git

- **Free and Open Source:** Git is available without purchasing a license.
- **Version History:** Developers can create commits and return to previous versions of their projects.
- **Offline Development:** Developers can commit changes and review project history without an internet connection.
- **Branching and Merging:** Developers can experiment with new features without directly affecting the main project.
- **Fast Operations:** Most Git operations are performed locally.
- **Collaboration:** Multiple developers can work on the same project and combine their changes.

### Cons of Git

- **Learning Curve:** Git commands and workflows can be difficult for beginners and non-programmers to understand.
- **Large File Handling:** Git is not optimized for frequently changing large binary assets, although Git LFS can help.
- **Binary File Conflicts:** Files such as textures, models, and audio cannot always be merged automatically.
- **File Locking:** Git does not include built-in file locking, although Git LFS provides locking functionality.
- **Repository Size:** Large projects with extensive file histories can require significant storage space.

### Git in Game Development

Git is useful in game development because programmers and artists often need to collaborate on the same project.

For example, in a Unity project:

- Programmers can track changes to C# scripts and game mechanics.
- Team members can create branches to develop new features independently.
- Developers can restore earlier versions if a new feature introduces bugs.
- Artists can manage textures, models, and audio files, although large assets may benefit from Git LFS.

Git is especially useful for managing code, but game development teams should consider how they will handle large binary files and merge conflicts.

### Git vs. GitHub

Although Git and GitHub are often used together, they serve different purposes.

- **Git:** A version control system that tracks and manages changes to files.
- **GitHub:** An online platform that hosts Git repositories and provides additional tools for collaboration.

Git can be used entirely on a local computer without GitHub.

GitHub provides features such as pull requests, code reviews, and remote repository hosting that make collaborating with others easier.

## Additional Resources

- [Pro Git - About Version Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- [Pro Git - What Is Git?](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F)
- [GitHub Docs - About Git](https://docs.github.com/en/get-started/using-git/about-git)
- [Pro Git - A Short History of Git](https://git-scm.com/book/en/v2/Getting-Started-A-Short-History-of-Git)
- [GitHub Docs - About Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage)
- [Unity Documentation - Unity Version Control](https://docs.unity.com/en-us/unity-version-control)
- [Perforce - Helix Core](https://www.perforce.com/products/helix-core)

## Team Member Biographies

<!--
Each team member must add their own short paragraph biography
to this section through a separate feature branch and pull request.

Add biographies below this comment.
-->
### Riley Clarke

Hi! My name is Riley, and I'm a Game Development – Programming student at RRC Polytech. I've been programming games in Unity with C# for just over five years, contributing to both 2D and 3D projects. I have a passion for programming, game design, and creating memorable and impactful experiences.

Outside of game development, I enjoy rock climbing, music of many genres, JDM cars, and, of course, playing video games!

My long-term goal is to establish my own game development studio, where I can create games that others will love and enjoy while providing employment opportunities for other passionate creatives.  
  

### Alex Poolie

Hi, my name is Alex Poolie. I am in the programming side of the game development program at rrc. Ever since I was able to play video games I have known
that I wanted to make them. I am primarally self taught, learning lua and autohotkey on my own. I have taken the first term of the AD&D program at rrc to learn python,
and oop. I love creating, and making worlds for people to explore.

I am also a self taught pianist, I love piano improvisation. Eventually my goal is to make music for games that I create.

My dream is to buy the rights to a game on roblox called "Rogue lineage", and turn it into a real game.  
  
  
### Traigen Skoropata

Intergalactic salutations! My name is Traigen, and I am a Game Development – Programming student at RRC Polytech. Outside of school, I also work as a line cook at Little Bones Wings.

I've been programming in Unity using C# and Python since Grade 10, giving me around four years of experience. I've worked on several solo game projects, taking on both programming and art responsibilities due to me not really working with anyone else. Although I took a break from programming after high school, I'm now continuing to develop my skills. Above all, I love storytelling and narrative in video games.

Outside of game development, I'm passionate about soccer (or football, if you're European), cooking (despite still having plenty to learn and sucking at it), Warhammer 40K/fantasy.

My long-term goal is to create a fantasy game with a powerful, tear-jerking story and memorable characters. I want players to feel as though they've formed genuine friendships with the characters they meet throughout their journey. Ultimately, I hope to create a game that leaves a lasting emotional impact on the people who play it.  
  

### Gus Klaverkamp

Hello, my name is Gus. I am a Programming and Game Design student at RRC Polytech. I have been programming and making games since just before high school and I learned how to use unity in Sisler Create. I enjoy the prospect of creating interesting games and the possibility of telling interesting and engaging stories within those games. 

Outside of game development, I am currently in the middle of writing a graphic novel that has been in the worlds for 10+ years called Guardian. I also like to draw and am versed in character design and concept art. 

My long term goal is to publish said book and share my stories with the world. 

That and maybe taking over the tri-state area I guess.  

### Nova Acosta

Greetings, my name is Nova Acosta. I go by she/her. I am part of the Game Design - Programming course at RRC. I've always loved video games and codind. I took 3 years of Computer Science in high school and attended Sisler CREATE for game design for 1 year.

Due to my time at Sisler CREATE, I have become pretty familiar with Unity and C#. I have made a couple of small games both solo and in groups and one big game over the span of around 10 months.

As for my interests outside of game development, I of course love video games. Big fan of ULTRAKILL, rhythm games, fighting games, puzzle games, a lot of stuff. I also really like music, specifically FLAVOR FOLEY and Ado. If you see me with headphones on,
I'm probably listening to one of those two. 
  
