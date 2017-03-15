# IIS
## Reports
* Administration Reports
* FastTrack Reports
* IA Reports
* QualityStage Reports

## istool
You can use the istool commands to manage assets that are stored in the metadata repository of IBM IIS. 

Command                | Description  
-----------------------|-------------  
istool export          | Export assets to a file
istool import          | Import assets from a file
istool glossary export | Export assets from IBM InfoSphere Business Glossary to a file
istool glossary import | Import glossary assets from a file
istool build package   | Build a package of IBM InfoSphere DataStage and QualityStage assets to be deployed
istool deploy package  | Deploy a package
istool send package    | Send a package to the local client computer
istool query           | Query common metadata (implemented data resources, logical and physical data models, and business intelligence assets) and write the results to a file
istool deletecm        | Delete common metadata
istool delete          | Delete InfoSphere DataStage and QualityStage assets

### istool export/import
Import/Export the following types of assets:
* Common metadata assets: using `-commonmetadata` parameter
  - Implemented data resources: `export -dom 192.168.168.90:9443 -username isadmin -password isadmin -archive "C:\Users\jian\istool_workspace\commonmetadata_archive.isx" -commonmetadata '/PAVAN90/XE/ESTUATE/*.tbl'`
  - Business intelligence (BI) assets
  - Physical data model assets
  - Data connections
  - Contract libraries
* Custom attributes
* Data Click assets
* InfoSphere DataStage and QualityStage assets
* FastTrack assets
* Information Analyzer assets
* IGC extended data sources and extension mapping documents
* IMAM artifacts
* InfoSphere Streams assets
* Logical data model assets
* MDM models
* Reporting assets
* Security assets

## Update IIS from 11.5 to 11.5.0.1
* Download **11.5.0.1 Fix Pack 1** and **Update Installer 11.5.1.93** (prerequisite): https://www-945.ibm.com/support/fixcentral/swg/downloadFixes?product=ibm/Information+Management/IBM+InfoSphere+Information+Server&function=fixId&fixids=is115_fp1_server_client_win&includeRequisites=1&includeSupersedes=0&downloadMethod=http&login=true
* Install Update Installer: unzip and copy to `C:\IBM\InformationServer\Updates`
* Use Update Installer install Fix Pack 1: 
  - cmd(admin): `cd C:\IBM\InformationServer\Updates\bin` `installUpdates.exe` 
  - use Update Installer to install patch `fixpack_FP1_IS115_windows_11500.ispkg` (1.1GB)
  - Application Server Administrator: wasadmin/wasadmin
