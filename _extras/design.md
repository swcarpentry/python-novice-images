---
layout: page
title: "Lesson Design"
permalink: /design/
---

## Contents
{:.no_toc}

* Jekyll will replace this line with an auto-generated table of contents.
{:toc}

> ## Help Wanted
> {:.no_toc}
>
> **We are filling in the exercises [below](#stage-3---learning-plan)
> in order to make the lesson plan more concrete.
> Contributions (both in the form of pull requests with filled-in exercises,
> and comments on specific exercises, ordering, and timings) are greatly appreciated.**
{: .callout}

## Process Used

This lesson was developed using a slimmed-down variant of the "Understanding by Design" process.
The main sections are:

1.  Assumptions about audience, time, etc.
    (The current draft also includes some conclusions and decisions in this section - that should be refactored.)

2.  Desired results:
    overall goals, summative assessments at half-day granularity, what learners will be able to do, what learners will know.

3.  Learning plan:
    each episode has a heading that summarizes what will be covered,
    then estimates time that will be spent on teaching and on exercises,
    while the exercises are given as bullet points.

## Stage 1: Assumptions

*   Audience
    *   Graduate students in numerate disciplines from cosmology to economics
    *   Who are sighted
    *   And have manipulated data in spreadsheets and with interactive tools like SAS
    *   But have *not* programmed beyond CPD (copy-paste-despair)
*   Constraints
    *   One full day 09:00-17:00
        *   06:30 teaching time
        *   1:00 for lunch
        *   0:30 total for two coffee breaks
    *   Learners use native installs on their own machines
        *   May use VMs or cloud resources at instructor's discretion
        *   But must keep native local install as an option
    *   No dependence on other Carpentry modules
        *   In particular, must not require knowledge of shell or version control
    *   Use the Jupyter Notebook
        *   Authentic tool used by many instructors
        *   There isn't really an alternative
        *   And means that even people who have seen a bit of Python before will probably learn something
*   Data
    *   Use and create images throughout
*   Focus on NumPy and scikit-image.
    *   Makes lesson usable by both carpentries
    *   Image processing appeals to almost everyone
    *   Useful for people with some prior experience:
        *   will accept image processing as an authentic task
        *   but are unlikely to have encountered  it,
            so they'll still get something useful out of the lesson
*   Exercises will mostly *not* be "write this code from scratch"
    *   Want lots of short exercises that can reliably be finished in allotted time
    *   So use MCQs, fill-in-the-blanks, Parsons Problems, "tweak this code", etc.
*   Lesson materials
    *   Notes for instructors and self-study will be written in Markdown
        *   We've tried writing/maintaining lessons as Notebooks...
    *   Learners will be provided with one Notebook per episode containing exercises

## Stage 2: Desired Results

### Questions

How do I...

*   ...read and display an image?
*   ...manipulate the pixels in an image?
*   ...automate these tasks?
*   ...write programs I can understand a week from now?

### Skills

I can...

*   ...write short scripts using loops and conditionals.
*   ...write functions with a fixed number of parameters that return a single result.
*   ...import libraries using aliases and refer to those libraries' contents.
*   ...read, write, and manipulate images.

### Concepts

I know...

*   ...that a program is a piece of lab equipment that implements an analysis
    *   Needs to be validated/calibrated before/during use
    *   Makes analysis reproducible, reviewable, shareable
*   ...that programs are written for people, not for computers
    *   Meaningful variable names
    *   Modularity for readability as well as re-use
    *   No duplication
    *   Document purpose and use
*   ...that there is no magic: the programs I use are no different in principle from those I build
*   ...how to assign values to variables
*   ...what integers, floats, strings, and NumPy arrays are
*   ...how to trace the execution of a `for` loop
*   ...how to trace the execution of `if`/`else` statements
*   ...how to create and index lists
*   ...how to create and index NumPy arrays
*   ...how to manipulate the pixels in an image
*   ...the difference between defining and calling a function
*   ...where to find documentation on standard libraries
*   ...how to find out what else scientific Python offers

## Stage 3: Learning Plan

### Summative Assessment

*   Midpoint: create thumbnails for all the images in a directory.
*   Final: blend two images.

### Running and Quitting Interactively (09:00)

*   Teaching: 15 min (because setup issues)
*   Exercises: 0 min (accounted for in teaching time - no separate exercise)
    *   Run the Notebook
    *   Create a few Markdown cells
    *   Create and execute a Python cell that prints 1+2

### Variables and Assignment (09:15)

*   Teaching: 10 min
*   Exercises: 10 min
    *   Trace behavior of three-step swapping
    *   Calculate elapsed time in seconds using named values for seconds per minute, etc.

### Displaying Images (09:35)

*   Teaching: 10 min (because paths and file download)
*   Exercise: 10 min (because of display issues)
    *   Load and display

### Resizing Images (09:55)

*   Introduces tuples and `object.member` notation
*   Teaching: 10 min
*   Exercises: 10 min
    *   Load, resize, save

### Loops (10:15)

*   Using `for pixel in image`
*   Teaching: 15 min
*   Exercises: 15 min
    *   Remove all red
    *   Create a scaled wash (green depends on X or Y coordinate)

### Coffee: 15 min (10:45)

### Conditionals (11:00)

*   Teaching: 15 min
*   Exercises: 15 min
    *   Resize picture so that either height or width is 100px
    *   Keep largest of three color values (conditional in loop)

### Lists (11:30)

*   Teaching: 15 min (introduce `glob.glob`)
*   Exercises: 15 min
    *   Filter list of filenames to keep PNGs
    *   Create thumbnails for all files in a list

### Lunch: 60 min (12:00)

### Writing Functions (13:00)

*   Teaching: 20 min
*   Exercises: 20 min
    *   Extract and encapsulate thumbnailing (image and size as parameters)
    *   Encapsulate again (take directory path as input, loop)

### Documentation (13:40)

*   Teaching: 10 min
*   Exercises: 10 min
    *   Add docstrings to functions written earlier

### NumPy Arrays (14:00)

*   Teaching: 20 min
*   Exercises: 15 min
    *   Create images with blocks of color

### Coffee: 15 min (14:35)

### Testing (14:50)

*   Teaching: 15 min
*   Exercises: 15 min
    *   Write function(s) to satisfy a set of assertions

### Python Scripts (or, life outside the Notebook) (15:20)

*   Teaching: 15 min
*   Exercises: 15 min
    *   Read text file specifying images and sizes and create thumbnails

### Wrapping Up: 10 min (15:50)

### Finish (16:00)
