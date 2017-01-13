# InfoSphere Metadata Asset Manager
## Topology Diagram
The components of IMAM are distributed across multiple tiers. Components are installed automatically on the services and repository tier, and manually on the client tier. 

### Repository Tier
* Staging Area
* **Metadata Repository**: you can export assets, browse and search for common metadata assets, set implementation relationships between them, and merge duplicates. 

## Common Metadata Assets
* Implemented data resources, such as database tables and data files
* Physical data model assets, such as design tables and design columns
* Logical data model assets, such as logical entities, entity attributes, and relationships
* Business intelligence (BI) assets, such as BI models, BI collections, and BI reports that are based on database tables
* Data connections and custom attributes

## Security Roles
* **Common Metadata Administrator**: delete metadata. 
* **InfoSphere Metadata Asset Manager**: allow deletion of import areas that were shared to the repository. 

## Tasks 
### Import 
Where you analyze and preview the contents of the import in a staging area before you share it to the metadata repository. 
#### Import Tools
IMAM uses the following types of import tools:
* **InfoSphere Metadata Integration Bridges**, which import metadata from many types of tools, files and databases, including IBM Cognos, CA ERwin, InfoSphere Data Architect, HDFS, InfoSphere MDM, and SAP BusinessObjects. 
* **IIS connectors**, which import database metadata from databases such as Amazon S3, Greenplum, Teradata, Oracle, Netezza, and DB2, and by using ODBC and JDBC connections. 

### Repository Management
Where you find, inspect, manage, and export assets that are in the metadata repository. 

### Administration
Where you set import policies and manage the metadata interchange servers where bridges and connectors are installed. 
