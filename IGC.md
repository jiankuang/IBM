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
* A **Collection** is a group of differnet types of assets that are brought together for analysis or for a common business context. 
* We can add both business glossary and information assets even collections into collection. 
* Collection can have multiple owners. 
* Collection can have multiple child collections. 
* Collection can be put in multiple parent collections. 
* Collections can be searched by Name, Short Description, Long Description, Labels, Modified Time. 
* Collections can be shared through Visilibity. 
* Shared Users can edit collection, even add themselves as Owners. **Not sure this is a good design!!!**
* Collection modification doesn't go through Workflow. (Workflow only works on Business Glossary)
