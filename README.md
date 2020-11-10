# ConnectALL SAP/Solman Adapter

ConnectALL SAP/SolMan Adapter is developed as an extension to the Universal Adapter capability of ConnectALL. The adapter specifications will let the user sync a SolMan incident using a custom api developed in SolMan to another endpoint using the ConnectALL Integration Hub. A custom api must be developed in SOlMan (an example is included in this repository). A common use if that SolMan minotring detects an alert, the alert exceeds a pre-defined threshold (like 10% disk left), and the incident is sent to an issue tracking suystyem (ITSM) like JIRA or ServiceNow where the alert is worked, resolved, and the status of Done/Closed is sent back to SolMan.

Please refer to https://wiki.connectall.com/ca/latest/user-guide/adapters/custom-application-adapter for more information

# How to use

## Import specifications
* Import solman_config.zip into ConnectALL using "Install custom adapter" feature.
* Create a custom api in SOlMan that will implement a rest api that ConnectAll will poll for new incidents.

## Define application links
* Create an application link in ConnectALL between AolMan and a destination application of your choice
* Navigate to `Configuration -> Connections` screen and create a new connection to SolMan.
* In the Entity mapping tab under Advanced Properties choose "Sync Type" as POLL

> In order to use the SolMan adapter you will need to get the license from ConnectALL sales team. Please reach out to sales@connectall.com for licenses and quotes.

