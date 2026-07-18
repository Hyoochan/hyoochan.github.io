---
title: "Project : Linux_to_do_list software (Retrospective)"
description: "Retrospective about Linux_to_do_list software"
date: "2026-07-18"
categories: [Project, Software, Linux-to-do-list, Retrospective]
tags: [project, software, retrospective]
---

# Project : Linux_to_do_list [Retrospective]

## 1. Why I Built Linux_to_do_list software?
> On July 4, 2026, I installed Pop!_OS on my main coumputer. I had a lot of tasks to do, so I needed a to-do-list app and I found "endeavour".
> It was heavy and uncomfortable to use. So I decided to build my own CLI_to_do_list software

## 2. Log
![Image1](/assets/img/Screenshot_2026-07-04_23-27-10.png)
![Image2](/assets/img/Screenshot_2026-07-04_23-30-59.png)

Image1 was my first code on my project. but It doesn't work. and I learned that if I want to use **continue** command It must be on While loop.
so I fixed  as Image2.

![Image3](/assets/img/Screenshot_2026-07-04_23-55-52.png)

I needed to save the todo-list data. because I need to see it later. So I updated code as Image3.

But, It's uncomfortable to execute python code every time so I made bash script.

![Image4](/assets/img/Screenshot_2026-07-05_00-00-28.png)

Image4 was first bash script. But changes was limited to the active terminal window.
So I chaged to save the bash script to ~/bashrc (Image5).

![Image5](/assets/img/Screenshot_2026-07-05_00-10-35.png)

It was saved. But changes didn't applied to the terminal.
So I added source ~/.bashrc to apply to the terminal(Image6). 

![Image6](/assets/img/Screenshot_2026-07-05_00-20-06.png)


## 3. Next Steps for Linux_to_do_list Project
- **Task Deletion**: A feature to select and delete a task from to-do-list
- **Dynamic Task Entry**: A feature to enter tasks without limits until the user quits

## 4. Reflections on My Development Habits
- ** Variable Naming** : I need to name variable more Meaningful.
- **Architecture Before coding (Designing First)** : I must design first before coding 
