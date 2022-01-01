---
layout: post
title: "Assembly programming vs. programming in high-level languages"
image: /blog_assets/programming-unsplash.jpg
hero_image: /blog_assets/programming-unsplash.jpg
hero_darken: true
---

>When you’re studying computer science, not all courses are going to be equally interesting or important. 
Eventually, there are bound to be some classes that teach things that are now obsolete.

I thought that programming in assembler is going to be one of those things, but I was wrong.

Learning about how complicated programming used to be, gives you perspective. Now, of course, the purpose of the class 
is not to teach us all to be successful assembly programmers, that would be silly. The idea of the course is to teach 
students how computers work, and how much they advanced. For example, now, it is trivial to add up two numbers in 
high-level programming languages, but how many lines of code it needed to be done in the assembler? Let’s take a look:

<figure align="center">
    <img src="/blog_assets/c+++assembler.png">
    <figcaption align="center">Comparison of two programmes that have the same purpose</figcaption>
</figure>

In the first programme, there is not much to explain, the syntax is clear: **‘int main()’** is the main function, **‘a’** and 
**‘b’** are variables type integer, **‘;’** is a delimiter, and **‘return 0’** is there to return the value of the main function.

Now, in the second programme, we have a little more commands that don’t seem very understandable at first.

**‘START’** initialises the beginning of the programme.

**‘ORG’** defines the memory address from which the next value starts. So, **‘ORG $1000’** just sets the current address to 
$1000 meaning the following store label will be at that address.

**‘LEA’** stands for Load effective address, so **‘LEA.L B, A0’** loads effective address of B to A0.

Command **‘MOVE.L (A0), D0’** moves A0 to D0, and because D0 is privileged, A0 needs to be in round brackets.

**‘ADD.L #5, D0’** adds number 5 to D0.

Command **‘TRAP #15’** pushes PC (Programme Counter) and SR (Status Register), PC set by vector table #15, and the range of 
numbers here can go from 0 to 15.

**‘DS’** stands for define space, and **‘DS.B 4’** defines space for 4 bytes.

**‘END’** signifies the ending of the programme, similarly like ‘return 0’ in C++.

Here is how the programme looks in the simulator **“Motorola 68 000”**:

<figure align="center">
    <img src="/blog_assets/before.png">
    <figcaption align="center">Before starting the programme</figcaption>
</figure>

<figure align="center">
    <img src="/blog_assets/after-adding-5-D0.png">
    <figcaption align="center">Programme after adding 5 to D0</figcaption>
</figure>

<figure align="center">
    <img src="/blog_assets/after-executing.png">
    <figcaption align="center">Programme after executing</figcaption>
</figure>

##### Conclusion

As you can see, it was quite a job to make this programme running. The today development environment is much more 
user-friendly, with lots of built-in libraries. You don’t need a cheat-sheet with commands, every time you want to add 
or subtract two values. However, the assembler has an extraordinarily relevant role in programming, and technology 
itself. It made the leap from writing code in binary to machine coding, which lead to high-level programming languages 
we use today.