# Information Analyzer

## Scenarios for Information Analysis
### Data Quality Assessment Project
* To profile your data, you run column analysis, key and cross-domain analysis, and baseline analysis to evaludate the content and structure of the data. 
* The results from data profiling project can help you to determine whether you need to complete data cleansing tasks on your data by using **QualityStage**

## Different Types of Analyses
### Column Analysis
* After column analysis completes, a frequency distribution for each column is generated and then used as the input for the subsequent analyses. 
* Investigate -> Column Analysis

### Primary Key Analysis

### Foregin Key Analysis
Run a **key and cross-domain analysis** job, compare the primary key of one table to the columns of another table to determine if there is a relationship between the two tables. 

### Redundant Analysis
To determine if columns contain overlapping or redundant data, you can run a **key and cross-domain analysis** job across columns in one or multiple tables or sources. 

### Baseline Analysis
Compare the column analysis results for two versions of the same data source.   

## Configurations
### Roles
#### Suite Roles
* Suite Administrator: Provides maximum administration privileges throughout the suite. 
* Suite User: Provides access to the suite and to suite components. Default role. 

#### Suite Component Roles
* IA Data Administrator: Creating a data connection to the analysis database, Configure global analysis settings. 
* IA Project Administrator: Creating a project and configuring project-level settings. 
* IA User: Configure the project dashboard. 

#### Project Roles
* IA Business Analyst
* IA Data Operator
* IA Data Steward
* IA Drill Down User

### Project
Project creation process: Create project -> Add data sources -> Add users -> Configure options
#### Add Users/Groups
Overview -> Project Properties -> Users/Groups -> Browse

### Jobs
When multiple analysis jobs are sent for processing, they are processed in a **queue**. 

### Published Rules
Develop -> Data Quality
