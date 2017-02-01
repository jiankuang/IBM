# IGC
learning notes about IGC project and so on

# Business Glossary

## Category
Created by IGC Author

## Term
* One of the major reasons for having a glossary of terms is to apply the terms to company information assets. 
* Created by IGC Author

### Associated Terms
* Related Terms: can be used as a catch-all if none of the other more specific relationships apply. 
* Assigned Terms: not sure what is it???  

### Assigned Assets
Asset types include:
* Glossary assets, such as categories. It is strange Term can be assgiend to Category asset???
* Database assets, such as database tables
* Data File assets, such as data files and data file records
* Data quality assets, such as data rules. We have Rules implemented by Data Rules, why assign them to Terms???
* ETL assets, such as DataStage jobs  

# Information Assets

## External Assets
External Assets are defined by an IGC administrator. 

# Other Assets
## Labels
* A text string used to group a set of terms together. 
* Created by an IGC administrator. 
* Can be applied to assets by any IGC user with authoring authorization. 
* Label modification doesn't go through Workflow. 

## Collections
* A **Collection** is a group of different types of assets that are brought together for analysis or for a common business context. 
* We can add both business glossary and information assets even collections into collection. 
* Collection can have multiple owners. 
* Collection can have multiple child collections. 
* Collection can be put in multiple parent collections. 
* Collections can be searched by Name, Short Description, Long Description, Labels, Modified Time. 
* Collections can be shared through Visilibity. 
* Shared Users can edit collection, even add themselves as Owners. **Not sure this is a good design!!!**
* Collection modification doesn't go through Workflow. (Workflow only works on Business Glossary)

## Lineage Reports
### Data Lineage Reports
* **Data lineage reports** show the movement of data through a job or multiple jobs. 

### Business Lineage Reports
* **Business lineage reports** show a simplified view of lineage that highlights the transformation and aggregation of data that is needed by a business user. 
* A user of IBM Glossary Anywhere and external programs such as IBM Cognos, can create a business lineage report for an asset. 


# Administration
## Setup
### Custom View
* Customize the order of properties in the Details page of some asset types (Term, Category, Rule, Policy). 
* Each Asset Type can only have one Custom View.
* Custom View is shared by all users. 

### Language Setting
* Specify the language for the user interface and for catalog content. 
* If you turn off Chinese in language setting for catalog content, you cannot search Chinese term. 
* Catalog content support for English is always on, even if you turn it off. 
* You can still create Chinese term even if catalog content support for Chinese is truned off, but you can't specify it as Chinese term. 
* Turning off Chinese content support will turn off terms specified as Chinese but not Chinese term specified as undefined Language.

## Lineage Management
### Manage Lineage Filters
Create and share filters that can be applied to data lineage and business lineage reports. 

# Update
## Update IGC Rollup 6 Patch 
http://www-01.ibm.com/support/docview.wss?uid=swg21996466  

* Update IIS from 11.5 to 11.5.0.1 (see IIS.md)
* Install ISF Rollup 5 version 2: https://www-945.ibm.com/support/fixcentral/swg/selectFixes?&product=ibm/Information+Management/IBM+InfoSphere+Information+Server&function=fixId&fixids=is11501_isf_ru5
* Install IIS Data Integration Rollup 1: http://www-01.ibm.com/support/docview.wss?uid=swg24043187 
* Install the patch for APAR JR56569: https://www-945.ibm.com/support/fixcentral/swg/selectFixes?product=ibm/Information+Management/IBM+InfoSphere+Information+Server&release=All&platform=All&function=fixId&fixids=is115_JR56569_XML_engine_client_all
* Install the patch for APAR JR56733: https://www-945.ibm.com/support/fixcentral/swg/selectFixes?product=ibm/Information+Management/IBM+InfoSphere+Information+Server&release=All&platform=All&function=fixId&fixids=is11501_JR56733_ccgui_client_win

* Install Governance Rollup 6: https://www-945.ibm.com/support/fixcentral/swg/downloadFixes?product=ibm/Information+Management/IBM+InfoSphere+Information+Server&release=All&platform=All&function=fixId&fixids=is11501_JR56838_IGC_services_engine_client_multi&includeRequisites=1&includeSupersedes=0&downloadMethod=http
