# So, you think you want to be a data scientist?

## What is data science?
I follow [Mason and Wiggins (2010)](http://www.dataists.com/2010/09/a-taxonomy-of-data-science/) and define data science as OSEMN...

1. Obtaining data
2. Scrubbing data
3. Exploring data
4. Modeling data
5. Interpreting data

...a good data scientist needs to be able to do all of these things well and this first-year undergraduate course would teach the foundational concepts and tools that a data scientist would use in order to accomplish steps 1-3 in the above data analysis pipeline.  While the second-year and third-year courses would cover the entire data analysis pipeline (using increasingly sophisticated tools/techniques) the focus of these courses would be on steps 4 and 5 (particularly in the third-year course). Idea is that after completion of all three courses, a student should be capable of successfully completing a substantive data science project as an honours thesis.

## Course syllabus

This course would teach the foundational concepts and tools used by a data scientist: Unix shell, version control, and programming. Familiarity with these concepts and tools will necessary in order to take courses 2 and 3.

I covered most of this material in the first 3 days of the computational methods workshop. The idea is that I would cover largely the same foundational material but at a *much* slower pace befitting an audience of first year undergraduates. I would also re-write, where necessary, the Software Carpentry lecture material in order to better motivate the example use-cases for an economic audience.  All example use cases would involve grabbing raw economomic data from the web, cleaning the raw data, and some *basic* exploratory data analysis (i.e., descriptive statistics and data visualization).

Students would be expected to bring their own computers to class. Ideally I would like to have a ["flipped classroom"](https://en.wikipedia.org/wiki/Flipped_classroom): I would assign readings, video lectures, and problem sets for students to cover on their own outside of class; lectures meanwhile would focus entirely on practical applications.

## Shock and awe (week 1)
The first week of the course would be spent impressing students with all of the cool things that they will learn how to do during the course.

## Unix Shell (weeks 2-4)
The Unix shell has been around longer than most of its users have been alive. It has survived so long because it’s a power tool that allows people to do complex things with just a few keystrokes. More importantly, it helps them combine existing programs in new ways and automate repetitive tasks so that they don’t have to type the same things over and over again. Effective use of the shell is so fundamental to data science that [Jeroen Janssens](http://jeroenjanssens.com/) has written an entire book called [*Data Science at the Command Line*](http://datascienceatthecommandline.com/) on how to use the shell and command line programs that extend it.  Use of the shell is also a pre-requisite for using a range of other powerful tools and computing resources (including “high-performance computing” supercomputers) that are widely used in industry. These lessons will start students on a path towards using these resources effectively.

### Topics covered

1. [Introducing the Shell](http://swcarpentry.github.io/shell-novice/00-intro.html)
2. [Files and Directories](http://swcarpentry.github.io/shell-novice/01-filedir.html)
3. [Creating Things](http://swcarpentry.github.io/shell-novice/02-create.html)
4. [Pipes and Filters](http://swcarpentry.github.io/shell-novice/03-pipefilter.html)
5. [Loops](http://swcarpentry.github.io/shell-novice/04-loop.html)
6. [Shell Scripts](http://swcarpentry.github.io/shell-novice/05-script.html)
7. [Finding Things](http://swcarpentry.github.io/shell-novice/06-find.html)

I would re-write all of the motivating examples in lessons 6 and 7 to make use of material from [*Data Science at the Command Line*](http://datascienceatthecommandline.com/) that is more economics focused.

## Programming using Python (weeks 5-8)
The best way to learn how to program is to do something useful, so this introduction to Python is built around a common scientific task: data analysis. The real goal isn’t to teach you Python, but to teach you the basic concepts that all programming depends on. I would use Python in my lessons because:

1. we have to use something for examples;
2. it’s free, well-documented, and runs almost everywhere;
3. it has a large (and growing) user base among scientists; and
4. experience shows that it’s easier for novices to pick up than most other languages.

The other obvious candidate would be *R*, however I think that teaching Python makes our students better prepared for the job market. The reality is that a good data scientists should be competent in both, and an expert in one or the other. Strong case for switching from STATA to R for econometrics.

![Python vs. R job growth](http://www.indeed.com/trendgraph/jobgraph.png?q=Python%2C+R&relative=1)

### Topics covered

1. [Analyzing Patient Data](http://swcarpentry.github.io/python-novice-inflammation/01-numpy.html)
2. [Repeating Actions with Loops](http://swcarpentry.github.io/python-novice-inflammation/02-loop.html)
3. [Storing Multiple Values in Lists](http://swcarpentry.github.io/python-novice-inflammation/03-lists.html)
4. [Analyzing Data from Multiple Files](http://swcarpentry.github.io/python-novice-inflammation/04-files.html)
5. [Making Choices](http://swcarpentry.github.io/python-novice-inflammation/05-cond.html)
6. [Creating Functions](http://swcarpentry.github.io/python-novice-inflammation/06-func.html)
7. [Errors and Exceptions](http://swcarpentry.github.io/python-novice-inflammation/07-errors.html)
8. [Defensive Programming](http://swcarpentry.github.io/python-novice-inflammation/08-defensive.html)
9. [Debugging](http://swcarpentry.github.io/python-novice-inflammation/09-debugging.html)
10. [Command-Line Programs](http://swcarpentry.github.io/python-novice-inflammation/10-cmdline.html)

I plan to re-write the motivating examples in the above Python lessons in order to show students how to use the [Pandas](http://pandas.pydata.org/) library to efficiently obtain and scrub data.  Time would also be spent on exploratory data analysis and visualization using browser-based Python plotting libraries (specifically, [Matplotlib](http://matplotlib.org/), [MPLD3](http://mpld3.github.io/), [plotly](https://plot.ly/), and [Bokeh](http://bokeh.pydata.org/en/latest/))

## Version control using Git and GitHub (weeks 9-10)
Version control is the lab notebook of the digital world: it’s what professionals use to keep track of what they’ve done and to collaborate with other people. Every large software development project relies on it, and most programmers use it for their small jobs as well. And it isn’t just for software: books, papers, small data sets, and anything that changes over time or needs to be shared can and should be stored in a version control system. Additionally, a GitHub profile has become the de-facto CV for anyone looking for a job as a data scientist.

![Git and Github job growth](http://www.indeed.com/trendgraph/jobgraph.png?q=git+and+github&relative=1)

### Topics

1. [Automated Version Control](http://swcarpentry.github.io/git-novice/01-basics.html)
2. [Setting Up Git](http://swcarpentry.github.io/git-novice/02-setup.html)
3. [Creating a Repository](http://swcarpentry.github.io/git-novice/03-create.html)
4. [Tracking Changes](http://swcarpentry.github.io/git-novice/04-changes.html)
5. [Exploring History](http://swcarpentry.github.io/git-novice/05-history.html)
6. [Ignoring Things](http://swcarpentry.github.io/git-novice/06-ignore.html)
7. [Remotes in GitHub](http://swcarpentry.github.io/git-novice/07-github.html)
8. [Collaborating](http://swcarpentry.github.io/git-novice/08-collab.html)
9. [Conflicts](http://swcarpentry.github.io/git-novice/09-conflict.html)
10. [Open Science](http://swcarpentry.github.io/git-novice/10-open.html)
11. [Licensing](http://swcarpentry.github.io/git-novice/11-licensing.html)
12. [Hosting](http://swcarpentry.github.io/git-novice/12-hosting.html)

