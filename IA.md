# Information Analyzer

## Scenarios for Information Analysis
### Data Quality Assessment Project
* To profile your data, you run column analysis, key and cross-domain analysis, and baseline analysis to evaludate the content and structure of the data. 
* The results from data profiling project can help you to determine whether you need to complete data cleansing tasks on your data by using **QualityStage**

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
* IA Drill Down User: specify the users who have permission to drill down to view the source data in your project. 

### Global Settings
#### Column Analysis Settings
* Nullability threshold
* Uniqueness threshold
* Constant threshold

#### Table Analysis Settings
* Primary key threshold
* **Composite key maximum**: Determine the maximum number of columns that can be combined when you search for primary key candidates. The range can be set between 2-32. 

#### Cross-table Analysis Settings
**Common domain threshold setting**: Determines the percentage of distinct values in the frequency distribution of one column that match distinct values in the frequency distribution of another column. If the percentage of matching distinct values is equal to or greater than the threshold, then the two columns are inferred to have a common domain. The default is 98%. 

### Project Settings
Project creation process: Create project -> Add data sources -> Add users -> Configure options
#### Project Environment
* **One or more Clients**: The client is connected to a **metadata repository**. The client is the interface that you use to complete tasks. 
* A Server
* **A Metadata Repository**: Stores all analysis work, configuration options, and analysis results. The repository is connected to data stores on a host computer through a **connector**. The metadata repository resides on the **server** computer.
* A Connector

#### Associating imported metadata with your project
Overview -> Project Properties -> Data Sources -> Add
#### Add Users/Groups
Overview -> Project Properties -> Users/Groups -> Browse
#### Analysis Settings
Overview -> Project Properties -> Analysis Settings -> Project

#### Enabling drill down security for a project
Once drill down security is enabled for a project, only users with the IA drill down project role can drill down into data. 
#### Customizing the project dashboard
* Getting Started pane
* Data Sources Summary pane
* Data Sources pane
* Completeness and Validity Summary pane
* Format Summary pane
* Property Summary pane
* Aggregated Anomalies Summary pane

### Jobs
When multiple analysis jobs are sent for processing, they are processed in a **queue**. 

### Published Rules
Develop -> Data Quality

## Managing Metadata
### Terms
Terms that are defined in IGC are available in IA and vice versa.  
Open IGC Category Hierarchy from IA: Home -> Metadata Management -> Terms -> Manage Term
#### Assigning assets to a term 
Terms -> Select a term -> Preview Term -> Assigned Assets -> Assgin New Asset
### Policies
Why Policies in IGC do not show in IA? They are different?
### Contacts
A contact contains personal information such as names, addresses, and telephone numbers of users. 
### Data Classes 
You can add a new data class to extend data classification and analysis capabilities. 

## Data Profiling Process
### Column Analysis
* Investigate -> Column Analysis
* After column analysis completes, a frequency distribution for each column is generated and then used as the input for the subsequent analyses such as primary key analysis and baseline analysis. 
* The column analysis process incorporates four analyses:

#### Domain analysis
#### Data classification analysis
* **Canadian SIN**: Infers whether a column can be considered a Canadian social insurance number (SIN). 
* **Code**: A column that contains code values that represent a specific meaning. For example, a column with the class of Code might contain data about the area code in a telephone number. 
* **Country Code**: Infers whether a column can be considered a country or region code. 

#### Format analysis
#### Data properties analysis

### Key and Cross-domain Analysis
During a key and cross-domain analysis job, your data is assessed for relationships between tables. 

#### Primary Key Analysis
#### Foregin Key Analysis
Run a **key and cross-domain analysis** job, compare the primary key of one table to the columns of another table to determine if there is a relationship between the two tables. 

#### Referential Integrity Analysis
* After a key and cross-domain analysis job completes, you can run a referential integrity analysis job on your data. 
* Referential integrity analysis is an analysis that you use to fully identify violations between foreign key and primary or natural key relationships. 

#### Redundant Analysis
* To determine if columns contain overlapping or redundant data, you can run a **key and cross-domain analysis** job across columns in one or multiple tables or sources. 
* If there are redundancies in your data, you might want to use a data cleansing tool to remove them because redundant data can take up memory and slow down the processes that are associated with them. 

### Baseline Analysis
Compare the column analysis results for two versions of the same data source.   

![Alt text](/IA_data_profilling_analyses.PNG?raw=true "IA Data Profilling Analyses")

# Citation
IBM InfoSphere Information Analyzer User's Guide.pdf 
