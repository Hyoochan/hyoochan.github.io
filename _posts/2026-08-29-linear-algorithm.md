--- 
title : "Implementing linear search algorithm"
description : "Implementing linear search algorithm with C"
date : 2026-08-29
categories : [Implementation, Algorithm]
tags : [implementation, algorithm, c, linear_search]
---

### Introduction
Hello! my name is Yoochan, I learned about linear algorithm on CS50 by havard 2019. And I just want to implement 
linear search algorithm. So, in this post I will implement linear search algorithm with C.
###### for education purpose
### Source Code

```c
#include <stdio.h>

int linear_search(int list[], int size_of_array, int t); //t is target number





int main(void)
{
        int t;
        printf("Enter target");
        scanf("%d", &t);
        int size_of_array;
        printf("Enter the size_of_array");
        scanf("%d", &size_of_array);
        int list[size_of_array];
        for (int j = 0; j < size_of_array; j++ )
        {
                printf("Enter the number");
                scanf("%d", &list[j]);
        }
        printf("founded index number : %d ", linear_search(list,size_of_array,t));


}









int linear_search(int list[], int size_of_array, int t) //t is target number
{
        for (int i = 0; i < size_of_array; i++)
        {

                if (list[i] == t)
                {
                        return i;
                }

                continue;
        }
        return -1;
}
```


### I learned
- 1. **How to get input: In CS50 I used get_(data_type) to get input. But in standard C enviroment, I need to use scanf**


