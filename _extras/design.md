---
layout: page
title: "Lesson Design"
permalink: /design/
---
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

While this looks like a waterfall process, in practice we did this:

1.  Draft the assumptions.

2.  Do one bullet point for each of several learning milestones.

3.  Draft the desired results.

4.  Update the learning milestones (still as just one bullet point each, no time estimates or exercises).

5.  Get early feedback from four people.

6.  Do a full pass to flesh out the assumptions and add time estimates and exercises.

7.  Ask for feedback and start iterating (mostly to cut things).

## Stage 0 - Assumptions

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

## Stage 1 - Desired Results

### Goals

1.  Learners can write short functions using loops, conditionals, and standard libraries.

### Summative Assessment

*   Midpoint: create thumbnails for all the images in a directory.
*   Final: blend two images.

### Essential Questions

How do I...

*   ...read and display an image?
*   ...manipulate the pixels in an image?
*   ...automate these tasks?
*   ...write programs I can understand a week from now?

### Learners Will Be Able To...

*   Run code interactively
*   Run code saved in a file
*   Write single-condition `if` statements
*   Write `for` loops to do operations on each element in a collection
*   Combine operations on basic data types (integer, float, string)
*   Call built-in functions
*   Use `help` and online documentation
*   Import a library using an alias
*   Call something from an imported library
*   Read and write image files
*   Manipulate NumPy arrays
*   Do whole-image operations (e.g., resize)
*   Do pixel-level operations on images (e.g., adjust color values)
*   Interpret common error messages
*   Write non-recursive functions taking a fixed number of named parameters
*   Create literate programs in the Jupyter Notebook

### Learners Will Know...

*   That a program is a piece of lab equipment that implements an analysis
    *   Needs to be validated/calibrated before/during use
    *   Makes analysis reproducible, reviewable, shareable
*   That programs are written for people, not for computers
    *   Meaningful variable names
    *   Modularity for readability as well as re-use
    *   No duplication
    *   Document purpose and use
*   That there is no magic: the programs they use are no different in principle from those they build
*   How to assign values to variables
*   What integers, floats, strings, and NumPy arrays are
*   How to trace the execution of a `for` loop
*   How to trace the execution of `if`/`else` statements
*   How to create and index lists
*   How to create and index NumPy arrays
*   How to manipulate the pixels in an image
*   The difference between defining and calling a function
*   Where to find documentation on standard libraries
*   How to find out what else scientific Python offers
