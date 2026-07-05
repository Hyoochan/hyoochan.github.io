---
title : "Project : Linux_to_do_list software [TechDocs]"
description : "Technical documentaion about linux_to_do_list software"
date: 2026-07-05
categories: [Project, Software, Linux_to_do_list, TechDocs]
tags: [project, software, techdocs]
---

# Project : Linux_to_do_list [TechDocs]

## 1. Why I Built Linux_to_do_list software?
> On July 4, 2026, I installed Pop!_OS on my main computer. I had a lot of tasks to do, so I needed a to-do-list app and I found "endeavour".
> It was heavy and uncomfortable to use. So I decided to build my own CLI_to_do_list software

## 2. Core features
* Add to-do-list : Quickly add new to-do-list
* Save to-do-list : Save to-do-list on Home directory
* Open to-do-list : Quickly open to-do-list

## 3. Tech Stack
* Python : Python 3.12.3
* Bash : GNU bash, version 5.2.21(1)
* Platform : Linux (Tested on Pop!_OS 24.04 LTS)

## 4. Developement Details

### 4-1. get_to_do.py
```python
from pathlib import Path

num = int(input())
def get_to_do_list():

	while True:

		to_do_list = []

		for i in range(0,num):
			to_do = input("Enter what you need to do : ")
			to_do_list.append(to_do)
		for list in to_do_list:
			print(list)
		answer = input("Is it right? [y/n] : ")

		if answer == "y":
			return to_do_list
		else:
			continue


final_to_do_list = get_to_do_list()
print("Your To-Do_List : " , final_to_do_list)

format_todo = "\n".join(final_to_do_list)

file_path = Path("./.todo.txt")
file_path.write_text(format_todo, encoding="utf-8")
```
- num = int(input()) : This code receive input by user. It is receving the input for the number of tasks.
- While True: : I used while loop to use **continue** command, because continue command needs to be inside of while.
- to_do_list = [] : It is a list for tasks
- 		for i in range(0,num):
			to_do = input("Enter what you need to do : ")
			to_do_list.append(to_do)
    : this code is reciving a tasks and appending to list(to_do_list)
-  		for list in to_do_list:
			print(list)
		answer = input("Is it right? [y/n] : ")
    : this code is asking if the list is correct
-
		if answer == "y":
			return to_do_list
		else:
			continue
    :this code is checking the input. If user enter "y" get_to_do_list() returns to_do_list. If user enter "n" get_to_do_list() continue.
- final_to_do_list = get_to_do_list() : save return value of get_to_do_list() on final_to_do_list
- print("Your To-Do_List : " , final_to_do_list) : print final_to_do_list
- format_todo = "\n".join(final_to_do_list) : It save as a new value with lines separated on format_todo
- file_path = Path("./.todo.txt")
file_path.write_text(format_todo, encoding="utf-8") : It creates file ./.todo.txt and write format_todo data on ./.todo.txt














