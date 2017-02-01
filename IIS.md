#IIS
## Reports
* Administration Reports
* FastTrack Reports
* IA Reports
* QualityStage Reports

## Update IIS from 11.5 to 11.5.0.1
* Download **11.5.0.1 Fix Pack 1** and **Update Installer 11.5.1.93** (prerequisite): https://www-945.ibm.com/support/fixcentral/swg/downloadFixes?product=ibm/Information+Management/IBM+InfoSphere+Information+Server&function=fixId&fixids=is115_fp1_server_client_win&includeRequisites=1&includeSupersedes=0&downloadMethod=http&login=true
* Install Update Installer: unzip and copy to `C:\IBM\InformationServer\Updates`
* Use Update Installer install Fix Pack 1: 
  - cmd(admin): `cd C:\IBM\InformationServer\Updates\bin` `installUpdates.exe` 
  - use Update Installer to install patch `fixpack_FP1_IS115_windows_11500.ispkg` (1.1GB)
  - Application Server Administrator: wasadmin/wasadmin
