# Pewlett-Hackard_Analysis
## Overview of the analysis: 
Bobby and I were tasked with setting up databases for Pewlett-Hackard to make employee csv data a bit more organized and set up Pewlett-Hackard for future success. In order to do so, we set up our data tables in an ERD - Entity Relationship Diagram. This diagram allowed Bobby and I to have a high-level view of the datatables and how they all connect. Our ERD for this task is below:

![PH-ERD](https://github.com/rmward17/Pewlett-Hackard_Analysis/blob/main/EmployeeDB.png)

Looking at the diagram, you can see the various datatypes and keys that connect the datatables. Using the ERD, we were able to create the tables in PostgreSQL and then import the csv data into the tables in SQL. Once all of the data was in place, we were able to create queries in order to get some key information about the future of Pewlett-Hackard. 

### Queries
Bobby and I ran a number of queries just to get a feel for the data. We looked at the number of emplyees that are eligible for retirement and retrieved the employee number, first name, and last name for each employeed born between 1952 and 1955 and hired between 1985-1988. We also wrote queries to export an employee information table, a list of managers per department, and a list of department information. Bobby and I did so well, that even the Sales Department wanted us produce a reitirment information for the Sales and Development teams as well.

Once we proved we could work wth SQL, we were tasked with creating two very important tables - the number of retiring employees by title and a table of employees eligible for a mentorship program. It took some time but we were able to produce both tables and export them to csv files for management.

Retiring Employees by Title      |  Mentorship Eligible Employees
:-------------------------:|:-------------------------:
![Unique Titles](https://github.com/rmward17/Pewlett-Hackard_Analysis/blob/main/unique_titles.png)|![Mentorship Table](https://github.com/rmward17/Pewlett-Hackard_Analysis/blob/main/mentorship_eligibility.png)

## Results: 
- There are only 5 active managers for 9 departments and 2 of them are retirement eligible 

![Retirement Title Count](https://github.com/rmward17/Pewlett-Hackard_Analysis/blob/main/count_by_title.png)

- Of the 72,458 retirement eligible employees, there are 1,549 people eligible for the mentorship program which is less than 2% of retiring employees
- There are no Managers that are mentor eligible 

![Mentor Title Count](https://github.com/rmward17/Pewlett-Hackard_Analysis/blob/main/mentor_by_title.png)

- Less than 6% of those retiring in all other position titles are eligible for mentorship

## Summary 
72,458 roles will need to be filled as a result of the "silver tsunami", ~30% of the total company. This is a huge percentage of company and quite concerning. The queries below allowed us to get the total number of employees and total number of retiring employees:

![query count](https://github.com/rmward17/Pewlett-Hackard_Analysis/blob/main/counts.png)

There are not enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees. There are only 1,549 potential mentors and 33,118 positions to be filled. It is a lofty expectation to have each person mentor 45-47 people. Perhaps an alternative solution would be for the mentors to develop training for these open postions so that each newly hired and promoted employee can have the value of the mentorship without putting too much on these retiring employees. I am sure management can come up with other solutions to this issue and we will support them with our analysis as best we can.
