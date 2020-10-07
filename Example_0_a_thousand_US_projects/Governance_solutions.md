## Selling Governance solutions

### Select a solution

Conversation establishes client features, notably:
1.  Aspiration: how big a change does the client want ?
2.  Landscape of current data and accountabilities

Use these to select a *path through the woods*. 

> *Example 1* Client just wants to get project delivery up and running. They have a relatively tidy situation: departments have few overlapping accountabilities. They want to push some change, but want pace to reflect current project maturity in setting a roadmap, so effort will be spread over several months. 

<image src="images1/Solution_selection_1.dot.png" width="270"/>

 We decide we can:
 
 1. take their excel stored data
 2. use a graph database to set up & populate a project-data model
 3. hand the data back in a relational database 
 4. Dashboard and views will be set up in PowerBI. 

*What are the features to select on ?*
*Which solution combinations work ?*

+++

## Implementation steps

| Steps                 |   Considerations                                            |
| ---------------------------------- | ---------------------------------------------                                               |
| Create_Reference_views                     |    Club agrees upfront                                          |
|    |..data model w accountabilities|
|    |..per maturity |
|    |..per sector |
| Map_against_reference_view     |    find a start-point                          |
| | from prelim discussions |
||add business entities|
| Identify_accountablities    |                                            agree key governance nodes|
||seed start-points for BIG|
|     |   complete for all entities|     
||define and describe| 
| Design_enablers                    |    enablers for Ops &BIG|   
||add governance, ops, data, MI |
||build around use cases|
||add relevant permissions|
||develop cadence, support,|
||develop methods and tools| 
| Design_data_to_insight_to_decision |     data provenance                                           |
||identify decision-capability [^*(e.g. performance, lifecycle step) assurance, analysis and problem solving, opportunity / threat discovery*] |
|| map data - insight |
|| map insight - decision|                                                                     
| Migration_stages_to_BIG            |   define stages                                          |
|| ..driven by business-need|
||..when entities switch across|
||..when data-base changes |
||..when data-links change |
| Design_enablers_for_growth       |  set integration roadmap                                             |
||identify emerging challenges|
||culture roadmap|

## Select Use-cases

| Origin  |      Use-case                                         |
| ---------- | --------------------------------------------- |
| one_we_design                 | Commercial reviews Supplier capacity        |
| one_that_emerges                | track un-managed dependencies               |
|                  | compare aspirations with actual dependencies|
|                                    |                                               |
|| etc.|


## When to use graphs
- we will need to go through several iterations with the client
- we want to use the data to generate the schema
- projects are only part of the picture
- data domains overlap 
- accountability is widely distributed

<image src="images1/Neo4j_features.jpg" width="270"/>


> 'graphs are naturally additive, meaning we can add new kinds of relationships, new nodes, new labels and new subgraphs to an existing structure without disturbing existing queries and application functionality'

**Indicators**

- delivery is not just done in projects
- staff are not just accountable for projects
- data items are shared across the enterprise
- accountabilities overlap

**Q: Is a graph database needed to generate graph visualisations ?**

*A: No. Most software allows you to do this. Graph databases do this natively, but this is not their main benefit*

+++

## Appendix 1 Two more examples

> *Example 3* Client xxxxxxx. 

<image src="images1/Solution_selection_3.dot.png" width="270"/>

 We decide we can:
 
 1. xx
 2. xx 

+++
## Appendix 2: example questions with client

**Questions about Aspiration**

- Do you just want to get things moving ?
- Are projects being delivered okay, but with unclear accountabilities ?
	- do you need to clarify accountabilities across all delivery?
	- will this be a fully funded initiative to set Governance?
	- this can be used to plan and drive change
	- otherwise, an incremental approach may be indicated
 - Are you needing to overhaul both delivery and governance ?
 - how would you describe your desired end-state ?

**Questions about Landscape** 

- how good is the data ?
- how well are the accountabilities working ?
- are data and accountabilities in silos or widely distributed ?
- is there a useful business logic within the data ?
- or is the delivery landscape simple and project-focussed ?
- if so, might a project-centric data-model work ?
- how would you characterise the as-is state ?

**Questions about Tools**

- where are the data stored ?
- how are we going to store the data we analyse ?
- how will we be providing the data back for Operations ?
- what will be the primary tool for ongoing visuals and analytics?