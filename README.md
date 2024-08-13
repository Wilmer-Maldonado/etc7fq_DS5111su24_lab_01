# etc7fq_journal_DS5111su24
Data Engineering UVA Grad Course

#### Status Badge

[![Python package](https://github.com/Wilmer-Maldonado/etc7fq_journal_DS5111su24/actions/workflows/validations.yml/badge.svg)](https://github.com/Wilmer-Maldonado/etc7fq_journal_DS5111su24/actions/workflows/validations.yml)

### Tokenizer Functions Documentation 

Collection of Functions that Process Strings

#### clean_text

description: takes a string as an argument, converts string to all lowercase and removes punctuation.

example use:

example_text = "Python. python. PYTHON HellO!,WorLd?."

clean_text(example_text) -> "python python python hello world"

#### tokenize

description: takes a string as an argument, returns a list of all the words in the string in lowercase form.

example use:

example_text = "Python. python. PYTHON HellO!,WorLd?."

tokenize(example_text) -> [python, python, python, hello, world]

#### count_words

description: takes a string as an argument, returns word count dictionary of the string.

example use:

example_text = "Python. python. PYTHON HellO!,WorLd?."

count_words(example_text) -> {"python": 3, "hello": 1, "world": 1}

### Journal Entries - Git O'reilly Textbook

May 28th, 2024 - Chapters 1 and 2 (Week 1 Journal)

- I've used the basic git commands before and have collaborated on projects with others using git for version control as well. 
The chapters were mostly a review but I enjoyed the visualizations and the 'why?' behind the structure of git. 
For example, the explanation of local repositories and their staging area and commit history.

June 10th, 2024 - Git Linux Command Line (Week 2 Journal)

- makefile is something that I have never done before. It was convenient and relatively simple how a single script could me made
to automate making multiple files. The format of naming each block in the script after the intended file name made for easy organization
and readable code. Navigating through the txt files with wget and local directory with only the command line took some getting used to, but 
it got easier the more I played around with being at different locations in the current working directory (pwd). This is where I found the reading 
most helpful, learning the commands that help navigate the directory via the shell and to find text that matches certain cases.

June 10th, 2024 - Python Marking/Cleaning Text and Logging (Week 3 Journal)

- This week 3 reading was mostly a review for me on how to use python functions to manipulate strings and search text for occurrences, counts of words or events.
What was new to me was how to log a file. It does make sense that to store all the logging messages it might be best to place them in a file to not lose track.
It seems like an ideal way to monitor usage and flag for errors that can be recorded in logs to later reference for debugging. 

June 17th, 2024 - Python tests

- For week 4 we went over the assert functions used in python tests functions and how pytest package is used to run test py scripts. 
This section was mostly a review since knew pytest and how to use assert function. What I did find helpful is how to modify pytest command 
to run only subtests of test.py if that's the only test I'm focused on testing/debugging code.

July 7th, 2024 - Github Workflow Automation

- For week 5 we went over github actions workflow via yaml files. I've ran github actions before but haven't created one from scratch. I know that developrs sometimes use these features to deploy and test code pipelines that might not be used for production but for analytics and tracking. The structure of worflow actions starts with the triggers named events. Components are jobs that have defined steps with runners deciding where the code will execute. I plan to catch up this week on the labs and quizzes I missed last week, and confirm I am setting up repo correctly for grading in office hours.

July 8th, 2024 - Creating python packages

- For week 6 we went over how to setup init.py, setup.py and a repo to make a pip installable package for python. I have had experience with making packages and virtual environments so this section was review. 

July 15th, 2024 - Decorators, Comprehensions, Dicts and some OOP

- For week 7, we learned about decorators that add/extend the behavior of a function by the operation defined by the dedorator. Comprehensions and Dicts were already review, as well as OOP.

July 20th, 2024 - Design Patterns

- For week 8, learned about Design patterns, specifically how Singleton, Factory, and Template designs work as examples. Never studied Design patterns specifically, but this aligns how I think about code. I always try to map the features to a diagram and design pattern of my own before I start coding a codebase or start making PRs. 

July 30th, 2024 - Database Design

- For week 9, I haven't gotten too far in the readings yet and working on the other labs. From what I have read database design is a structured format to be able to create read update delete information form a table in a consistent stable atomic way. 

August 1st, 2024 - Snowflake

- For week 10, I got to play around with snowflake. I've used databricks SQL query dashboard UI before and it was extremely similar to Snowflake. It was also interesting to learn how dbt interacts with snowflake and other backends. Snowflake is super common in job postings so I am glad we got cover its functionality.

August 8th, 2024 - Snowflake/DBT Part 2

- For week 11, took me sometime to figure out how to load the seed files and enter the inputs just right for dbt to login to snowflake. Once that was figured out it was easy to run dbt seed with the utf-8 encoded csv files. I had an error when I loaded a csv that was not utf-8 so that was a good learning lesson. Also learned that dbt init creates another folder in repo with all dbt connection configuration. 

August 9th, 2024 - Snowflake/DBT COntinued and AWS Logging

- For the final week, week 12 tried logging into AWS and running repo. Created the instance fine with the class account, but had trouble installing homebrew. I tried installing with only sudo commands python and everything worked fine. I was able to clone repo, make the environment and import my package from git successfully