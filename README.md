<!---

TASK LIST:

  * Use cp -rf *.* to copy all of the files and directories in this repository
    to the starter repository for this assignment
  * Change into the directory for the starer repository
  * Update the header (e.g., #) to only give the name of the assignment
  * Update the first paragraph to include the commented-out content
  * Change the link in the # Problems section to point to this lab's starter
  * Create the assignment in the GitHub Classroom, noting the URL
  * Test the assignment by accepting it with your own GitHub account
  * Check to ensure that your GitHub repository is created correctly
  * Share the assignment link with all of the students using email or Slack

PROBLEMS?

  * Contact Gregory M. Kapfhammer by email or Slack
  * Raise an issue in the GitHub repository for this assignment

-->

# cs101-F2018-practical9-starter

Designed for use with [GitHub Classroom](https://classroom.github.com/), this
repository contains the starter for Practical 9 in Computer Science 101. Since
the Travis builds for this repository will initially fail (as evidenced by a red
&#x2717; appearing in the commit logs instead of a green &#x2714;), the
programmer is responsible for completing all of the steps needed to satisfy the
requirements for the assignment, thus causing a &#x2714; to instead appear in
the commit logs.

## Introduction

This assignment requires a programmer to understand the methods in a `WordCount`
program that is inspired by the source code segment in Section 10.1.2 of the
textbook. With that said, the provided source code combines the `Tree` and and
`HashMap` data structures to implement a more comprehensive solution. Your job
for this assignment is to run the program and study its output. Then, you are
responsible for adding comments to the source code that demonstrate you
understand how the `WordCount` program uses both a `Tree` and a `HashMap` to
produce the expected output. You should also add the correct output statements
to the program's source code. Students who are interested in doing so are
encouraged to write extra Java methods that can, for instance, print out the
word that is most frequently found in the input file. Additionally, you are
invited to run the `WordCount` program with a different input file. Finally,
as verified by [Checkstyle](https://github.com/checkstyle/checkstyle), the
source code for all of the Java classes must adhere to all of the requirements
in the [Google Java Style
Guide](https://google.github.io/styleguide/javaguide.html).

When you use the `git commit` command to transfer your source code to your
GitHub repository, [Travis CI](https://travis-ci.com/) will initialize a build
of your assignment, checking to see if it meets all of the requirements. If both
your source code and writing meet all of the established requirements, then you
will see a green &#x2714; in the listing of commits in GitHub. If your
submission does not meet the requirements, a red &#x2717; will appear instead.
The instructor will reduce a programmer's grade for this assignment if the red
&#x2717; appears on the last commit in GitHub immediately before the
assignment's due date.

A carefully formatted assignment sheet for this project provides more details
about the steps that a computer scientist should take to complete this
assignment. You can view this assignment sheet by visiting the listing of
laboratories on the course web site.

## Learning

If you have not done so already, please read all of the relevant [GitHub
Guides](https://guides.github.com/) that explain how to use many of the features
that GitHub provides. In particular, please make sure that you have read the
following GitHub guides: [Mastering
Markdown](https://guides.github.com/features/mastering-markdown/), [Hello
World](https://guides.github.com/activities/hello-world/), and [Documenting Your
Projects on GitHub](https://guides.github.com/features/wikis/). Each of these
guides will help you to understand how to use both [GitHub](http://github.com) and
[GitHub Classroom](https://classroom.github.com/).

Please read all of the content and study all of the technical diagrams and
source code segments in Sections 8.1 through 8.3 and 10.1 through 10.2. Finally,
please see the course instructor or one of the teaching assistants or tutors if
you have questions about any of these reading assignments.

## Commands

To get started in using the GatorGrader tool, you can change into the directory
for this assignment and type the command `gradle grade` in your terminal.
Running this command will produce a lot of output that you should carefully
inspect. If the output indicates that GatorGrader judges that there are no
mistakes in the assignment, then this means that your source code and writing
are passing all of the automated baseline checks. However, if the output
indicates that there are mistakes, then you will need to understand what they
are and then try to fix them.

Running this command will produce a lot of output that you should carefully
inspect. If the last line of the output indicates that GatorGrader judges that
there are no mistakes in the assignment, then this means that your source code
and writing are passing all of the automated checks. However, if the last line
of the output indicates that there are mistakes, then you will need to
understand what they are and then try to fix them.

You can also complete several important Java programming tasks by using the
`gradle` tool. For instance, you can compile (i.e., create bytecode from the
program's source code if it is a correct program) the program using the command
`gradle build`. There are also additional commands that you can type:

- `gradle clean`: clean the project of all the derived files
- `gradle check`: check the quality of the code using Checkstyle
- `gradle build`: create the bytecode from the Java source code
- `gradle run`: run the Java program in the command-line
- `gradle cleanTest`: clean the JUnit test suite of derived files
- `gradle test`: run the JUnit test suite and produce report
- `gradle tasks`: display details about the Gradle system

To run one of these commands, you must be in the home directory for this
assignment where the `build.gradle` file is located. Then, you can type the
command in the terminal and study the output.

If the course instructor publishes a new version of GatorGrader and asks you to
access it, then you need change into the tool's directory by typing `cd
gatorgrader`. Then, you can type the command `git pull` to download the new
source code for the GatorGrader tool. If this command completes successfully,
then you can return to the main directory for this practical assignment by
typing `cd ..` and then continuing your work.

## Output

Instead of running an experiment, the `WordCount` program reads in a file and
then uses a combination of the `Tree` and `HashMap` data structures to analyze
the words that are in the file. The following output illustrates how the
specialize type of `HashMap` stores and outputs the key-value pairs associated
with the words and their word-count frequencies. Instead of asking you to write
code to produce this output, the assignment requires you to add comments to the
source code to demonstrate that you understand how the program works.

```
Reading and tracking the words in the file ...
... Finished reading and tracking the words in the file.

Analysis of the words in the file ...

(key, value) pairs sorted by key:

{a=4, already=1, append=1, associated=3, associates=1, be=1, combining=1,
create=1, either=1, example=1, for=2, function=1, given=2, if=2, is=3, it=1,
key=2, mapped=1, mapping=1, may=1, method=1, msg=1, multiple=1, non=1, not=1,
null=3, of=2, or=3, otherwise=1, remapping=1, removes=1, replaces=1, result=1,
results=1, specified=1, string=1, the=6, this=1, to=2, use=1, value=4, values=1,
when=1, with=4}

(key, value) pairs sorted by value and key:

[already=1, append=1, associates=1, be=1, combining=1, create=1, either=1,
example=1, function=1, it=1, mapped=1, mapping=1, may=1, method=1, msg=1,
multiple=1, non=1, not=1, otherwise=1, remapping=1, removes=1, replaces=1,
result=1, results=1, specified=1, string=1, this=1, use=1, values=1, when=1,
for=2, given=2, if=2, key=2, of=2, to=2, associated=3, is=3, null=3, or=3, a=4,
  value=4, with=4, the=6]

... Finished the analysis of the words in the file.
```

## Checking

Since this assignment asks you to write comments to explain an existing source
code segment, the checks for the practical will be performed directly by the
course instructor. You will receive the checkmark grade for this practical
assignment if your source code builds correctly, it produces the same output as
is given in the assignment sheet, and it has thoughtful comments that correctly
explain how each source code segment works.

## Updates

If the course instructor updates the provided material for this assignment and
you would like to receive these updates, then you can type this command in the
main directory for this assignment:

```
git remote add download git@github.com:Allegheny-Computer-Science-101-F2018/cs101-F2018-lab9-starter.git
```

You should only need to type this command once; typing the command additional
times may yield an error message but will not negatively influence the state of
your repository. Now, you are ready to download the updates provided by the
course instructor by typing:

```
git pull download master
```

This second command can be run whenever the course instructor needs to provide
you with new source code for this assignment. However, please note that, if you
have edited the files that the course instructor updated, running the previous
command may lead to Git merge conflicts. If this happens, you may need to
manually resolve them with the help of the instructor or a teaching assistant.

## Travis

This assignment uses [Travis CI](https://travis-ci.com/) to automatically run
the checking programs every time you commit to your GitHub repository. The
checking will start as soon as you have accepted the assignment, thus creating
your own private repository, and the course instructor enables Travis for it. If
you are using Travis for the first time, you will need to authorize Travis CI to
access the private repositories that you created on GitHub.

## Requirements

The GatorGrader software that supports the checking of this assignment was
developed for the following software and versions:

- Gradle 4.6
- Java 1.8.0
- JUnit 4.9.0
- MDL 0.4.0
- Proselint 0.8.0
- Python 3.6

## Problems

If you have found a problem with this assignment's provided source code, then
you can go to the [Computer Science 101 Practical 9
Starter](https://github.com/Allegheny-Computer-Science-101-F2018/cs101-F2018-practical9-starter)
repository and create an issue by clicking the "Issues" tab and then clicking
the green "New Issue" button. If you have found a problem with the [GatorGrader
tool](https://github.com/gkapfham/gatorgrader) and the way that it checks you
assignment, then you can follow the aforementioned steps to create an issue in
its repository. To ensure that your issue is properly resolved, please provide
as many details as is possible about the problem that you experienced. If you
discover a problem with the practical assignment sheet, then please raise an
issue in the
[cs101-F2018-sheets](https://github.com/Allegheny-Computer-Science-101-F2018/cs101-F2018-sheets)
repository and mention this assignment.

Students who find, and use the appropriate GitHub issue tracker to correctly
document, a mistake in any aspect of this practical assignment will receive
free laptop stickers and extra credit towards their grade for it.

## Assistance

If you are having trouble completing any part of this project, then please talk
with either the course instructor or a teaching assistant during the practical
session. Alternatively, you may ask questions in the Slack team for this course.
Finally, you can schedule a meeting during the course instructor's office hours.
