# A portfolio of 8 programmes managed in a graph database

## The Sub-portfolio held by the US FDA
The FDA Food and Drug Administration had 8 sets of investments:
- 3 are named programmes
- 5 are ongoing spend, and have not been named for simplicity

/images/*8_investments.png

The three programmes together have 17 projects

/images/17_projects.png

Each project has a number of tasks or activities, 122 over 17 projects. 

/images/project_activity.png

This is the schema, shown so far. 

/images/core_schema.png

In addition, we have shown above that Investments are judged for success by Metrics, or KPIs. Here are the metrics for one investment.

/images/metric.png
There are 52 metrics across the 17 investments. 

These investments are provided through 11 contracts held with 8 suppliers. For instance:

/images/supplier_contract.png

## The purpose of the investment programmes
At the Government level, there are 7 broad types of administrative service that have been defined which investments provide.
For the 3 programme investments in the FDA, they together serve two of these. 

/images/Services_to_investment.png

The US Government also has a hierarchy of overall policy and citizen outcomes, which all Government work is tied back to. The three investment programmes tie back to general Health and IT outcomes:

/images/business_function.png

## Properties
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

## Summary
Looking at the entire FDA portfolio, this is 232 nodes altogether, and 252 relationships between them.

/images/FDA_232_nodes.png

This is the overall schema, pulling together all the elements described above.

/images/schema.png

The FDA sub-portfolio described above is part of the broader Health Bureau.

# The Portfolio of the US Health Bureau

This Agency is responsible for the work of 11 Bureaus, of which one is the FDA: 

"Centers for Medicare and Medicaid Services"
"Health Resources and Services Administration"
"National Institutes of Health"
"Indian Health Services"
"Centers for Disease Control and Prevention"
"Department of Health and Human Services"
"Substance Abuse and Mental Health Services Administration"
"Administration for Children and Families"
"Agency for Healthcare Research and Quality"
"Departmental Management"
"Food and Drug Administration"

Altogether these Bureaus run 721 Investments, of which many are Programmes, the remainder being Operational spend. 

There are 202 Projects run to deliver these Programmes, and 1102 Activities described within these Projects. 

These investments are judged by 455 Metrics.

These investments contribute to 18 Business Functions, grouped into three business areas: 
The top five contributions are to:
- "Health" supported by 	338 investments 
- "IT Management" supported by 136
- "Planning and Budgeting"	 supported by 37
- "Controls and Oversight"supported by 	34
- "Administrative Management" supported by	32

These investments contribute to 29 Business Functions. The top five contributions are to:
- "Knowledge Management"	supported by 185 investments
- "Management of Process"	by 138
- "Financial Management"	 by 60
- "Tracking and Workflow"	by 40
- "Development and Integration"	by 30


Here we look at which Suppliers are used three times or more 

/images/Suppliers_used_3_times.png

Overall, there are 2796 nodes representing these features of the Health Agency, along with 3677 relationships between them, plus additional properties related to each node as described above for the FDA. 

