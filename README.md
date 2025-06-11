# cs6238-project-i-solved
**TO GET THIS SOLUTION VISIT:** [CS6238 Project I Solved](https://mantutor.com/product/cs6238-project-i-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;113047&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6238 Project I Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
&nbsp;

Learning Objectives:

The goal of this project is to help students become familiar with memory protection facilities provided by operating systems. In particular, you will learn how to limit access to a certain region of memory (e.g., only read, write or execute access). The project has two parts. First, you will learn about mprotect(), a memory protection system call. In the second part, you will explore why it is a good idea to disable execution on the stack to safeguard a program’s execution. Memory protection is not limited only to these two examples, there are many different methods to protect the stack and heap. You are encouraged to look at and familiarize yourself with other relevant memory protection mechanisms as well. However, to keep this project simple and of limited scope, we will focus only on the protection of the memory by the above two discussed mechanisms. Thus, the objectives of the project are as follows:

1. Understand how mprotect() works and how it can be implemented.

2. Understand the benefits of turning off the executable stack.

Project Setup:

Note: The link to the VM will be posted on a Piazza pinned post.

For this project, you will be provided an Ubuntu-based Virtual Machine (VM). This VM was tested on Oracle VM Virtual box 5.2.16 and can be directly imported to it . This VM has a default account “project1” setup with normal user access privileges. You do not need root account credential for completion of this project.

Password for the “project1” account is “CS6238”. You should not include “” while entering the password. When you log into account “project1”, you will find Project_1 folder on Desktop. This folder contains 2 additional folders named, Stack_Protection and M_protect. We are going to use the contents of folder M_protect for completion of Task 1, and similarly contents of Folder Stack_Protection for Task 2.

Background:

This project assumes that you know the basics of C programming language (or can learn it quickly). More specifically, you should be able to understand and modify a given C code snippet. Second, you should know how a basic buffer overflow works. For the understanding of basic buffer overflow, you can refer to course materials in CS 6035, Intro to Information Security. If not, try some Google-fu.

Project Details: For both tasks, you should first do some exploration and then conduct specified experiments or answer some questions based on the learning. The project should be straightforward and is more focused on exploring things and how they work.

Task 1: Protection of Memory via mprotect() (50% of grade):

This task is divided into two parts, (A) Understanding mprotect(), and (B) Experimenting with programs that use this call. The understanding part is 40% of this task (i.e., 20% of the total grade of this project). The remaining 60% will be for the implementation and experimentation part of this task.

Part A) Understanding Memory Protection (20% of grade):

To answer:

1. Why do you get SIGSEGV when you execute the object code generated by compiling the mprotect.c program?

2. How does mprotect() protect memory ? What is the minimum size requirement for this call, what happens if you pass the value of the “len” argument as 1?

3. Sam is a programmer and he needs to protect a 0x380 byte block starting at memory address 0x1234000 and ending at address 0x1234379. This block should be protected from overwriting by some other internal function. Can Sam use the mprotect() function in his C program to protect this memory space? Explain your answer.

4. Review and report what data is being protected in mprotect.c by the mprotect() function. Moreover, discuss if any function can perform read or write on the protected data. If the mprotect call is used in multiple instances, write your observations for each of them.

Part B) Experimentation and Implementation (30% of grade):

1. Write first n bytes of last two pages (9th and 10th page) with your first name where n is equal to number of characters in your first name.

2. Now, use mprotect() to allow read and write access on 7th and 8th page. Write your last name in first n bytes of 7th and 8th pages, where n is equal to number of characters in your last name and then try to read it. You should display it on output screen (print to STDOUT).

4. Now, create a buffer of 2 pages and try to copy 7th and 8th page into it. Can you copy it, if not why?

5. Now try to copy 6th page and 9th page into the previously created buffer. Are you able to do so? If not, when your code hit SIGSEGV, is it copying 6th or 9th page? Explain your answer.

All the above steps should be followed in the same order, and updates should be made to the same script.

Deliverables for Task 1:

1. Completed code (Exercise.c).

2. Report.pdf – Report.pdf should contain a section called Task 1 which should contain answers to the above asked questions for Part A and Part B.

Note: Do not zip up the deliverables. Upload them separately.

Task 2: Non-Executable Stack (50% of grade):

This task is also divided into two parts, (A) Understanding the importance of non-executable stack, and (B) Experimenting with vulnerable code with protected and unprotected stack. The understanding part is worth 60% of this task (i.e., 30% of total grade of this project). The remaining 40% is for part B.

Part A) Understanding Stack Protection (30% of grade):

Review various mechanisms that are used to protect against buffer overflow exploits. More specifically, research the methods given below and write a brief explanation for each one of them. Each answer must be no more than a paragraph, and definitely no more than half a page of text (diagrams do not count to this limit).

1. Stack smashing via buffer overflow.

2. Stack canary.

3. NX (Non-Executable Stack).

4. Address space layout randomization (ASLR).

Part B) Experiments with execution of code (20% of grade):

For this part of task 2, you need to locate the Stack_Protection directory via terminal, and there you will find vuln.c. You should review it carefully and then compile this source code into four different binaries with the following gcc options:

• gcc -g -O0 -fno-stack-protector -z execstack -o vuln-nossp-exec vuln.c

• gcc -g -O0 -fno-stack-protector -o vuln-nossp-noexec vuln.c

• gcc -g -O0 -z execstack -o vuln-ssp-exec vuln.c

• gcc -g -O0 -o vuln-ssp-noexec vuln.c

Task 2 Part B Questions:

(Each answer should be no more than a paragraph.)

1. Explaining the functionality of -fno-stack-protector and -z execstack options of gcc. Explain the differences you see in the binaries when the binaries are created with and without these options.

2. Which of the above four binaries can you exploit, by smashing the stack and overflowing a buffer?

3. Attempt to find the stack canary value in vuln-ssp-exec binary, by using a debugger like gdb.

Does the canary value change or remain the same across multiple compilations/ executions? Post screenshots of your attempts. Deliverables for Task 2:

1. Report.pdf. The same Report.pdf should also contain a section – Task 2, which has your answers of the above asked questions in Task2, for Part A and Part B and screenshots/ diagrams if required.

Note: Just a single Report.pdf for both Task1 and Task2! Good luck!
