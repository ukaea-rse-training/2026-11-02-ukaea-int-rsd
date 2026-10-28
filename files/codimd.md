# Intermediate Research Software Development in Python

**Date:** November 2026

:::info
This document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents. It is written in a markup language called Markdown, which you will learn about more in the course. You shouldn't need to do any fancy formatting, so for the most part treat it like a regular text document. There is a cheatsheet you can access by clicking the '?' in the top bar, and there are rich editing features at the top of the editing pane.

Users are expected to follow our **[Code of Conduct](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html)**.

All content is publicly available under the [Creative Commons Attribution License](https://creativecommons.org/licenses/by/4.0/).
:::

[TOC]

## General Information

Any problems in advance or that require discretion, please email [Harry Saunders](mailto:harry.saunders@ukaea.uk). During sessions, you can privately message helpers or the instructor through MS Teams.

Course Content: https://carpentries-incubator.github.io/python-intermediate-development/index.html

Workshop Website: [https://github.com/ukaea-rse-training/2026-11-02-ukaea-int-rsd](https://github.com/ukaea-rse-training/2026-11-02-ukaea-int-rsd)

Installation Instructions: please consult the Workshop Website immediately above.


## Day 1

### Attendance List


1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 

### Setting the Scene For the Workshop


### Section 1: Setting Up Environment For Collaborative Code Development


### Introduction to Our Software Project

#### :pencil2: Obtain the Software Project Locally

#### :pencil2: Have a Peek at the Data

_Which command(s) would you use to list the contents or a first few lines of `data/inflammation-01.csv` file? Please enter your answer below. Wrap code in triple back-ticks to get formatting. Let's see your unix-shell-fu!_

```bash
# put your answer under here


````

#### :pencil2: MVA Applications from Your Work (skipped)


### Virtual Environments For Software Development

#### :pencil2: Creating a `venv` Environment

_Read through to the end of the page and follow along with coding examples._


#### Exporting/Importing Virtual Environments Using `pip`

Some further reading on what should go in `requirements.txt` and whether to pin dependencies:

- <https://packaging.python.org/en/latest/discussions/install-requires-vs-requirements/>
- <https://caremad.io/posts/2013/07/setup-vs-requirement/>
- This scientific Python cookiecutter syncs `requirements.txt` and `install_requires` in `setup.py`: <https://github.com/ukaea/scientific-python-cookiecutter>

If you need to scrap your environment and create a new one:

```bash
rm -r venv/
python3 -m venv venv
source venv/bin/activate
pip install <your_dependencies> 
# or
pip install -r requirements.txt  # great reason to have this file
```

### Integrated Software Development Environments


#### :pencil2: Using the PyCharm IDE

_Read along and follow with your IDE to the end of the page._


### Collaborative Software Development Using Git and GitHub

#### :pencil2: Checking-in Changes to Our Project

_Start from this heading and go until the "Git Branches" heading._


#### :pencil2: Creating Branches

_Please read and complete the material to the end of the page._


### Python Coding Conventions

#### Style in Other Languages

- C++
  - [`clang-format`](https://clang.llvm.org/docs/ClangFormat.html) is widely used for enforcing formatting, and there are [built-in presets](https://clang.llvm.org/docs/ClangFormatStyleOptions.html#configurable-format-style-options) for existing conventions followed by Google, LLVM, etc. Project specific settings made in a `.clang-format` file.
  - our guide on C++ for VSCode recommends cpplint: https://intranet.ccfe.ac.uk/software/guides/vscode-cpp.html
  - Some other useful resources that cover a broader scope than just style and formatting are [Google's C++ Style Guide](https://google.github.io/styleguide/cppguide.html#Formatting) and the [C++ Core Guidelines by Bjarne Stroustrup (the creator of C++)](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md)
- Fortran
  - we have a great guide on tooling in VSCode: https://intranet.ccfe.ac.uk/software/guides/vscode-fortran.html
  - this is a good online resource: https://fortran-lang.org/learn/best_practices

#### :pencil2: Indentation

_Please read and complete the material to the end of the page._

### Verifying Code Style Using Linters

#### :pencil2: Exercise

_Read from the top of the page to the bottom, completing exercises as you go._

### Feedback Day 1

#### What went well?

-

#### What didn't go so well?

## Day 2

### Attendance List

1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 

### Section 2: Ensuring Correctness of Software at Scale

### Automatically Testing your Software

#### :pencil2: Set Up a New Feature Branch for Writing Tests

Question 1: Testing scope: what is the correct order of these different types of tests if they should be in ascending order of scope (i.e. the amount of the code base they cover)

1. end-to-end, functional/integration, unit
2. functional/integration, unit, end-to-end
3. unit, functional/integration, end-to-end
4. unit, end-to-end, functional/integration

Answers 1:

1.
2. 
3. 
4. 

Question 2: Automated testing of our code is important because (select all that apply)

1. it can quickly help anyone verify that the code is working the way that the developer intended it to
2. it provides a harness in which we can make changes to the code and be more sure that these changes do not alter behaviour of the code that shouldn't change
3. it reduces the overhead of new developers trying to determine if the code works on their machine
4. all of the above
5. none of the above

Answers 2:

1. 
2.
3.
4. 
5.


### Scaling Up Unit Testing

#### :pencil2: Parameterising Our Unit Tests

In the last 5-7 minutes, please think about the question: _Where can and might the input data and corresponding expected results come from for code you use in your usual work?_ Record answers here. Feel free to discuss with your peers.



#### Limits of Testing

[Some further thoughts](https://bielsnohr.github.io/2021/11/29/iccs-part2-and-testing.html) about what level and type of testing researchers should aim for.

### Continuous Integration for Automated Testing

#### :pencil2: Continuous Integration with GitHub Actions

### Diagnosing Issues and Improving Robustness

#### :pencil2: Start from the top of above page

### Feedback Day 2

#### What went well?

- A positive part of the lesson...
-
-
-

#### What didn't go so well?

- An aspect of the lesson that could be improved...
-
-
-

## Day 3

### Comments From Last Section


### Section 2 Progress

#### CI Episode:

Done: 
 
Not: 

#### Debugging Episode to Defensive Programming:

Done: 

Not Done: 

### Attendance List

1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 

### Section 3: Software Architecture and Design

#### Features of good and bad code

Good:

- ?

Bad:

- ?


####  Software Architecture and Design

##### Group Exercise: What is bad about this code?

- E.g., its formatting makes it hard to read.

#### Progress with regression test

Done: 
Not Done: 


#### Feedback Day 3

##### What is one thing you learnt

- 
- 
- 
- 

##### What one thing would you like more details on

- 
- 
- 
- 

##### What went well?

- 
- 
- 
- 
- 

##### What didn't go so well?

- 
- 
- 
- 
- 

## Day 4

### Attendance List

_Please add your name, UKAEA email address, and role to the list. You can use emojis if you are in the mood by typing `:` and then searching through the dialog._

1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 


#### Progression with regression test

Done: 
Not done: :japanese_goblin:

### Feedback Day 4

#### One Up
- 
- 
- 
- 
- 
- 
#### One Down
- 
- 
- 
- 
- 


## Day 5

### Attendance List

1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 


### Section 4: Improving and Managing Software Over its Lifetime


Start from the top of this episode page and read through to the end.

#### Other Technical Documentation

This is a nice overview of how to think about the different types of documentation: https://documentation.divio.com/

#### Choosing an Open Source Licence

The RSE team has some guidance specific to UKAEA about licensing: https://intranet.ukaea.uk/software/guides/intellectual-property-and-licensing.html

## Day 6

### Attendance List

1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 
1. 

### Quick Demo: Merge Conflicts!

### Continue Section 4

#### Preparing Software for Reuse


####  Packaging Code for Release and Distribution


### Section 5: Managing and Improving Software Over Its Lifetime



#### Assessing Software for Suitability and Improvement

Start reading from the top of this episode page all the way to the end. Complete exercises as you go.

You will need to synchronise as a group at the **🖉 Decide on your Group’s Repository!** exercise. Please use a sticky/reaction to indicate when you have reached this exercise.

For the next exercise, you will then need to wait for the other group you are assessing to fill in their repo URL.

##### :pencil2: [Decide on your Group's Repository!](https://ukaea-rse-training.github.io/python-intermediate-development/43-assessing-software-suitability-improvement/index.html#decide-on-your-groups-repository)

| Group Name | Repository URL   | Group that you will assess |
| ---------- | ---------------- | -------------------------- |
| MAST-U     |                  |                            |
| JET        |                  |                            |
| STEP       |                  |                            |

#### Software Improvement Through Feedback

##### Breakout: Start from the Top

Start reading from the top of this episode page all the way to the end. Complete exercises as a group.


### Wrap-up

## Appendices

Links to other tools and items of interest mentioned during the course

- [`git switch` and `git restore` vs `git checkout`](https://github.blog/2019-08-16-highlights-from-git-2-23/#experimental-alternatives-for-git-checkout)
- [VS Code Extension for seeing review comments](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)

## Contact Us
If you have any more questions or want to discuss anything the RSE team holds weekly consultation sessions every Thursday at 10am (in person near Costa or virtually if preferred). There is a dedicated Teams channel for announcements [here](https://teams.microsoft.com/l/channel/19%3a11d3f3a8e47945178fe70b2e14cff8c0%40thread.skype/RSE%2520Consultation?groupId=6b1c9009-c40d-4806-82fe-803b66367929&tenantId=c6ac664b-ae27-4d5d-b4e6-bb5717196fc7). You are also welcome to drop us an email:
* harry.saunders@ukaea.uk
* matthew.bluteau@ukaea.uk

:::info
**Post-course Survey: insert link**
:::
