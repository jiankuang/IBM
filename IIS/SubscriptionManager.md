# Notification Types
## Email 
Email notifications are sent to you. You can specify that **other suite users** receive copies of the email. 

### Configuring an email provider
To use Subscription Manager to send email notifications to users, you must specify and configure the email server that is used. 

## Application 
* An application is a software program or routine that takes a specific action when it is notified of the event.
  - For example, an application might start a process to notify users of a change to an exception that occurred in a data rule.
* Notification is sent to a program that processes notices of events. 
* Not all event types support applications. Some support only email notification. 
* Applications that send events to IBM Business Process Manager require that you specify the credentials of an IBM BPM user. 
* Applications that send events to an IIS suite tool or product do not require credentials. 
* Applications for exception event types are provided with the installation of **IBM® Stewardship Center**.

### Create and Register an Application
* You can create your own application in **IBM Business Process Designer**
* then register it to an exception event type by using the `istool event registerCallback` command
  - Specify a description for the application by using the `callbackDescription` option so that users of Subscription Manager understand what the application does. 
* When you no longer need a process, you can remove it by using the `istool event unregisterCallback` command. 
  - The process is removed from Subscription Manager and you need to delete any subscriptions that use the removed process.
  
### Sample processes in the application
When you install **Data Quality Exception Console**, the following sample processes are installed and registered, and subscriptions that use the processes are automatically created.

#### Data Quality Exception Console
When a NEW_EXCEPTIONS_EVENT is generated, a preexisting subscription to the process ensures that all new exception sets appear in Data Quality Exception Console.

#### IBM Stewardship Center - Data Quality Exception
IBM Stewardship Center - Data Quality Exception is a sample process that sends exceptions sets from Data Quality Exception Console to IBM Stewardship Center to be managed.
  
# Subscriptions
* Two subscriptions are created automatically when you install **Data Quality Exception Console**, one subscription for each exception event type. 
* You must have the role of IIS Suite Admin to see and delete those subscriptions. 

# Cited 
https://www.ibm.com/support/knowledgecenter/en/SSZJPZ_11.5.0/com.ibm.swg.im.iis.event.doc/topics/application_reference.html
