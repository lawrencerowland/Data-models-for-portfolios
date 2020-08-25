# A project portfolio at three levels

Here is a sample of what this covers:

/images/1_programme_in_1_Agency.png

Our graph database holds information about the whole portfolio of IT projects in US Government in 2013. 

Altogether the database holds management information about 1547 Projects, spread across 26 Agencies. 

One of these is the Health Agency which has:
- 202 Projects 
- spread across 11 Bureaus

One of these is the FDA (Food & Drug), which has
	- 17 Projects

I will describe the portfolio at the lowest level first, working up to the Government level. 

## The Sub-portfolio held by the US FDA
The FDA Food and Drug Administration had 8 sets of investments:
- 3 are named programmes
- 5 are ongoing spend, and have not been named for simplicity

/images/*8_investments.png

The three programmes together have 17 projects

/images/17_projects.png

+++

Each project has a number of tasks or activities, 122 over 17 projects. 

/images/project_activity.png

This is the schema, shown so far. 

/images/core_schema.png

+++

In addition, we have shown above that Investments are judged for success by Metrics, or KPIs. Here are the metrics for one investment.

/images/metric.png
There are 52 metrics across the 17 investments. 

These investments are provided through 11 contracts held with 8 suppliers. For instance:

/images/supplier_contract.png

+++


## The purpose of the investment programmes
At Government level, 7 types of business service have been defined. The 3 FDA programmes together serve 2 of these. 

/images/Services_to_investment.png

The US Government also has a hierarchy of policy/citizen outcomes. The FDA programmes deliver Health & IT outcomes:

<image src="/images/business_function.png" height="150"/>

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

# The Portfolio for the Department of Health and Human Services

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

This Health portfolio described above is part of the entire US Government Portfolio 

# The Portfolio of the US Government

The US Government is responsible for the work of 26 Agencies Bureaus, of which one is Health Agency discussed above. 
-437 Investments/programmes
-1547 Projects
-3827 Activities

-706 Suppliers
-1402 Contracts
-3462 Metrics/KPIs

Contribution to the Govt effort is defined across
-32 Business functions
-30 Services

One can ask questions across these 18728 nodes. 
For example, we are interested those Investment Programmes which deliver a 'Knowledge Discovery' Service.
We want to know which Business Functions these programmes support:

/images/Bus_fns_for_one_particular_service.png

We can ask how much these investment programmes cost, answer £ Enhancement_spend_$m.

We discover what is worst scoring of these investment programmes in terms of CIO Evaluation score. the answer is 4 out of 5. We also see that 3 out of the 6 programmes have not been evaluated by their CIO. 

We then ask to find the any investment programmes with a score of 1 out of 5. 
There is 1, and we can explore its relationships. 

/images/programme_with_lowest_eval_score.png

# Data

/images/Source_of_IT_data.png