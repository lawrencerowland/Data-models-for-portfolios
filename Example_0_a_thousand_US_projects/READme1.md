## Questions to ask of a project portfolio

### How many programmes are dependent on our largest single supplier ?

IBM supplies 16 programmes across 9 departments

<image src="images1/IBM_supplier.png" width="500"/>


### What metrics are being used to control these particular programmes ?

- Mostly around reliability and availability
- some around service accessibility
- some around cycle-time

<image src="images1/IBM_metrics.png" width="300"/>

### Which programmes are given low scores by clients ?

Out of 437 programmes, 8 score badly.

And what types of service are these lesser programmes providing?
- Systems Management 
- Security Management

<image src="images1/Poor_eval_programme_services.png" width="250"/>

### What does the lowest scoring programme look like ?

The worst programme has 4 suppliers delivering 5 contracts, with a main project delivering an HR resource management solution. 

<image src="images1/programme_with_lowest_eval_score.png" width="300"/>

### How much money is being spent on similar HR programmes ?

There are 6 similar programmes, totalling £82m of capital spend

<image src="images1/7_HR_programmes.png" width="300"/>

### How much delay to projects on these programmes ?

A total of 7894 days delay spread across these 20 HR projects

<image src="images1/projects_for_HR_investments.png" width="300"/>

17 other  HR projects have experienced no delay. 

### What tasks are in the schedules of these delayed projects?
There are 22 activities/tasks listed for these delayed projects

<image src="images1/all_activities_on_delayed_projects.png" width="300"/>

### Are these tasks finishing late because they are started late ?
No. On average they only start 4 days late
Whereas the typical start delay across all 3827 activities is 1.5 days

### So which types of programmes have the worst delays?
- worst programmes have delays ~ 20 days 
Here are the slowest programme types

<image src="images1/delay_starts_per_programme_type.png" width="250"/>

### Show all of programmes of this programme  type

- 'Controls & Oversight' programmes have worst record
- Here are the 5 programmes and 38 activities of this type

<image src="images1/Programmes_of_type_Controls_Oversight.png" width="300"/>

### Which metrics are being met ?
Metrics are recorded under different Measurement_categories (e.g. 202-Process and Activities) and also show whether the Metric is being met or not. We could:

Is Measurement category a guide to which metrics are deemed successful by the CIO ?
what about metric success ?
### Business functions for one particular service

At portfolio level, 7 types of business service have been defined. 

- Which programmes are designed to provide Knowledge Discovery Services?
- 5 programmes provide this Service

The portfolio also has a hierarchy of policy/citizen outcomes. 
- What business functions are delivered by these 5 programmes?
- The programmes use this service to provide science services, environmental mgt and economic development. 

<image src="images1/Bus_fns_for_one_particular_service.png" width="300"/>

## Overall

This portfolio has 

–437 Investments/programmes
–1547 Projects
–3827 Activities

–706 Suppliers
–1402 Contracts
–3462 Metrics/KPIs

Strategic alignment is linked to 
–32 Business functions
–30 Services

These are delivered by 26 Departments organised into 81 Bureaus

### The work of 1 department

One department (or bureau) runs 12 projects, comprised of 94 activities within 4 investments, 2 of which are programmes. These are controlled by 16 metrics, using 5 suppliers on 6 contracts, delivering 3 types of service as 3 business functions.

<image src="images1/FDA_146nodes_155rels.png" width="300"/>

### Schema
Although there are 18,728 nodes and 28,771 relationships between them, to cover the entire portfolio, it is easy to pull out the sub-set of interest. 

Everything follows one simple pattern, as shown in the schema. 

Left to right shows who owns which activities. 

<image src="images1/schema.png" width="300"/>

# Set-up

- This data is managed in a neo4j database on a free service tier. 

- It was created by importing 7 spreadsheets. 

- Now it can manage the portfolio, updating as necessary. 

The pattern / schema comes from the data and the management style of the portfolio. 

# Flexibility
There is no fixed neo4j pattern.

So the pattern can be updated as the portfolio management matures, whilst reflecting the reality of what records have been kept.

Or the portfolio can be managed where it is now, and periodically imported into neo4j to gain insight.
It is quick to implement as there is no permanent project-data-model to sign-off. 

Implement what you have, manage the portfolio, and iterate the structure as the organisation learns what it wants.

## Other information can be stored as properties
Neo4j allows the user to add properties to both nodes and relationships. 
The following four key node types have additional property data attached to each instance, as follows:

| Investment | Project | Activity | Metric |
|:--|:--|:--|:--|
| Investment_type | Updated_Date | planned_Costs | Metric_results |
| Changes_to_Baseline | name | Actual_duration | ID |
| Identifier | Planned_Cost | output_type | Description |
| name | Project_delay | Start_Date_Planned | Measurement_category |
| Last_Baseline | Start_days_after_2000 | No_Child_Activity |  |
| Performance_Gap | Cost_Variance | name |  |
| Summary | Id | description |  |
| Business_Case | Planned_Duration | Actual_start_delay |  |
| Enhancement_spend_$m |  | Id |  |
| Evaluation_by_CIO |  | status |  |

### Data source 

Thanks for the data to @projsuccess from last year's excellent Project Hack,  and @OxfordSBS for this data on IT projects managed by the US Government, 2013-2018. 

<image src="images1/Source_of_IT_data.png" width="300"/>













 








 