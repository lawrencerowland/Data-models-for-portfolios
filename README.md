# PURPOSE

Use a graph database to maintain and visualise a portfolio of projects.

# WHEN TO USE THIS

See https://lawrencerowland.github.io/2020/05/07/Data-models-for-Project-Portfolios.html 

## Option 1: Use Yworks

This is a good way of getting started. It is very user-friendly and requires no code. It is all you need to do during design and set up of a portfolio. 

You will find you progress onto option 2 when you are actually managing the portfolio day-to-day. 

[here](x)

## Option 2: Use Neo4j

You do not need to be able to code right from the outset - as there are useful tools that allow you to set up the initial model.

[arrows](http://guides.neo4j.com/arrows)

 [spreadsheet-template](https://neo4j.com/blog/importing-data-into-neo4j-the-spreadsheet-way/)

These will build the code as you sketch out your portfolio. You will then be able to open it and query it in Neo4j.

To manage the portfolio, and fully query the portfolio, you will need to learn the query language Cypher, which is pretty similar to SQL. There is a good introductory course on Neo4j website, which probably took me 3 days of effort in all. 

[here](x)



# Suitable portfolio context
1. annual business planning process selects and updates the portfolio
2. portfolio of current projects identified
3. portfolio reports exhibit characteristic "tells" of bottom up activity 
4. client curious about emergent strategy

Possible "Tells" 

# Signs a portfolio data model is needed

## Scope
ghost projects
year by year rolling programmes
design projects with general budget for implementation
scope = benefits
change requests coming out at all angles
project / functional characterisation unstable

## Planning / Times
No common WBS structure

## Cost
Unit costs unavailable

## Resource
Key resources spread across several initiatives
the design staff are very requirements-focussed
the BAU staff are very agile-focussed

## Working with the top-down materials

classic portfolio base-line and selection
strategy contribution per project etc

## working from bottom-up
What does the bottom-up look like in a P3 space ?
what project staff are actually working on
what low level internal clients are saying to their project providers
what resistance to project progress looks like here
As-is rather than to-be

## Specific portfolio services

typical ideation & innovation service
typical portfolio review and selection service, with the first collection stage widened to include bottom-up, bringing
modified benefits / scope categories
new project proposals
recommended project removals ("that doesn't work")
New strategic control installation service for ongoing support

# Techniques
## bundle
crowd source ideation
categorise ghost projects, new work-packages & scope change requests
check shop-floor BAU messaging from client with high-level message
gather risk and dependency and EVENT data per project
map and categorise the emerging scope categories and cost pressures
## unbundle
analyse and rationalise the emerging scope / benefits relationships
analyse the relationships between common risks, dependencies and events
## discover

# Inputs, tools and outputs
## bundle
project list, progress reports, change requests, interviews
Ideation app (Spigit, Brightspark)
Updated Benefit and scope tree / graph


## ACKNOWLEDGEMENTS
https://www.yworks.com Free products YEd Live and YEd are a good entry level to seeing the portfolio relationships as a graph
https://neo4j.com provide Neo4j Desktop for running graph databases as a Community edition, along with a number of more sophisticated enterprise products. 



