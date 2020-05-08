# PURPOSE

Use a graph database to maintain and visualise a portfolio of projects.

Graph databases work well for portfolios where:
1. there are many dependencies between projects and programmes
2. the data model may need to added to or changed over time, because of the dynamic nature of the business. 
3. Internal teams see and use the portfolio data in very different ways, and the teams need the ability to show multiple views of the same projects. 

# USE CASES

1. Portfolio is new and team needs to move from whiteboard charts to a portfolio database that fits the business

2. Portfolio is working well, and recorded well either in spreadsheet, or relational database, or Project Management System. Team wants to gain insight into how projects and objectives relate to each other, and chooses to view the same data in parallel with a graph database

3. The Portfolio data model is no longer suitable for the type of new projects or current business environment. The portfolio is well recorded in spreadsheet, or relational database, or Project Management System, and the team wish to move their data across to a new data model using a graph database. 

# INTRODUCTION

# Data model ?

The data model is what project attributes are conistently recorded and tracked in a given portfolio. 
For example, most projects will have data recorded for Scope, cost and schedule. 

# Why data models matter

1. A portfolio can consistently record the same type of data for each project
2. Only relevant data is collected and recorded, avoiding bloat. 
3. The data model can be made relevant to the purpose of the portfolio. 

# Where is the data model ?
In most portfolios, the data model is either:
1. implicit, and more or less the list of project attributes in a project spreadsheet
2. implied by the project /portfolio management software used
3. explicit, as a visual diagram showing the layout of project attributes within a portfolio relational database
4. aspirational, comprised of whiteboard diagrams for a new project portfolio. 

# Typical status within companies

Typically, a portfolio data model is in one of the following states:
1. Over time, most projects have come record the same attributes
2. A data model and database has been designed based upon company needs
3. conflicted, where historical project records now do not sit well with the new projects being set up. 

## ACKNOWLEDGEMENTS
https://www.yworks.com Free products YEd Live and YEd are a good entry level to seeing the portfolio relationships as a graph
https://neo4j.com provide Neo4j Desktop for running graph databases as a Community edition, along with a number of more sophisticated enterprise products. 



