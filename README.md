# So you think you want to be a data scientist?

This course would teach the foundational concepts and tools used by data scientist: Unix shell, version control, programming, and database management. Familiarity with these concepts and tools will necessary in order to take courses 2 and 3.

I covered most of this material in the first 3 days of the computational methods workshop. The idea is that I would cover largely the same foundational material but at a *much* slower pace befitting an audience of first year undergraduates. I would also re-write, where necessary, the Software Carpentry lecture material in order to better motivate the example use-cases for an economic audience.  All example use cases would involve grabbing raw economomic data from the web, cleaning the raw data, and some *basic* exploratory data analysis (i.e., descriptive statistics oand data visualization).

Students would be expected to bring their own computers to class. Ideally I would like to have a ["flipped classroom"](https://en.wikipedia.org/wiki/Flipped_classroom): I would assign readings, video lectures, and problem sets for students to cover on their own outside of class; lectures meanwhile would focus entirely on practical applications.

## Unix Shell (weeks 1-3)
The Unix shell has been around longer than most of its users have been alive. It has survived so long because it’s a power tool that allows people to do complex things with just a few keystrokes. More importantly, it helps them combine existing programs in new ways and automate repetitive tasks so that they don’t have to type the same things over and over again. Effective use of the shell is so fundamental to data science that [Jeroen Janssens](http://jeroenjanssens.com/) has written an entire book called [*Data Science at the Command Line*](http://datascienceatthecommandline.com/) on how to use the shell and command line programs that extend it.  Use of the shell is also a pre-requisite for using a range of other powerful tools and computing resources (including “high-performance computing” supercomputers) that are widely used in industry. These lessons will start students on a path towards using these resources effectively.

### Topics covered

1. [Introducing the Shell](http://swcarpentry.github.io/shell-novice/00-intro.html)
2. [Files and Directories](http://swcarpentry.github.io/shell-novice/01-filedir.html)
3. [Creating Things](http://swcarpentry.github.io/shell-novice/02-create.html)
4. [Pipes and Filters](http://swcarpentry.github.io/shell-novice/03-pipefilter.html)
5. [Loops](http://swcarpentry.github.io/shell-novice/04-loop.html)
6. [Shell Scripts](http://swcarpentry.github.io/shell-novice/05-script.html)
7. [Finding Things](http://swcarpentry.github.io/shell-novice/06-find.html)

## Version control using Git and GitHub (weeks 4-5)
Version control is the lab notebook of the digital world: it’s what professionals use to keep track of what they’ve done and to collaborate with other people. Every large software development project relies on it, and most programmers use it for their small jobs as well. And it isn’t just for software: books, papers, small data sets, and anything that changes over time or needs to be shared can and should be stored in a version control system.

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

## Programming using Python (weeks 6-8)
The best way to learn how to program is to do something useful, so this introduction to Python is built around a common scientific task: data analysis. The real goal isn’t to teach you Python, but to teach you the basic concepts that all programming depends on. I would use Python in my lessons because:

1. we have to use something for examples;
2. it’s free, well-documented, and runs almost everywhere;
3. it has a large (and growing) user base among scientists; and
4. experience shows that it’s easier for novices to pick up than most other languages.

The other obvious candidate would be *R*, however I think that teaching Python makes our students better prepared for the job market.

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

## Relational databases (weeks 9-10)
Three common options for storage are text files, spreadsheets, and databases. Text files are easiest to create, and work well with version control, but then we would have to build search and analysis tools ourselves. Spreadsheets are good for doing simple analyses, but they don’t handle large or complex data sets well. Databases, however, include powerful tools for search and analysis, and can handle large, complex data sets. These lessons will show how to use an SQL database to explore balance sheet data for U.S. banks.

While SQL (and perhaps relational databases in general) are stll widely used in industry...

![SQL vs. NoSQL jobs](http://www.indeed.com/trendgraph/jobgraph.png?q=SQL%2C+NoSQL)

...the use of SQL databases declining relative to NoSQL databases is declinging rapidly.

![SQL vs. NoSQL job growth](http://www.indeed.com/trendgraph/jobgraph.png?q=SQL%2C+NoSQL&relative=1)

My current plan is to cover NoSql databases in the 3rd year course. A solid understanding of SQL databases will help students understand when and why one should prefer SQL or NoSQL for a particular problem.

### Topics covered

1. [Selecting Data](http://swcarpentry.github.io/sql-novice-survey/01-select.html)
2. [Sorting and Removing Duplicates](http://swcarpentry.github.io/sql-novice-survey/02-sort-dup.html)
3. [Filtering](http://swcarpentry.github.io/sql-novice-survey/03-filter.html)
4. [Calculating New Values](http://swcarpentry.github.io/sql-novice-survey/04-calc.html)
5. [Missing Data](http://swcarpentry.github.io/sql-novice-survey/05-null.html)
6. [Aggregation](http://swcarpentry.github.io/sql-novice-survey/06-agg.html)
7. [Combining Data](http://swcarpentry.github.io/sql-novice-survey/07-join.html)
8. [Data Hygiene](http://swcarpentry.github.io/sql-novice-survey/08-hygiene.html)
9. [Creating and Modifying Data](http://swcarpentry.github.io/sql-novice-survey/09-create.html)
10. [Programming with Databases](http://swcarpentry.github.io/sql-novice-survey/10-prog.html)
