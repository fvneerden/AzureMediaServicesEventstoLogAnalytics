# AzureMediaServicesEventstoLogAnalytics
Store Azure Media Services Events in Azure Log Analytics

Azure Media Services v3 emits events on [Azure Event Grid](https://docs.microsoft.com/en-us/azure/media-services/latest/media-services-event-schemas). You can subscribe to these events in many ways and store the events in various data stores. In this tutorial we will subscribe to these events using a [Log App Flow](https://azure.microsoft.com/en-us/services/logic-apps/). The Logic App will be triggered for each event and store the body of the event in Azure Log Analytics. Once the events are in [Azure Log Analytics](https://docs.microsoft.com/en-us/azure/azure-monitor/learn/quick-create-workspace) we can use other Azure services to monitor, dashboard and alert on these events as desired by your own needs.

For this tutorial we expect you already have an [Azure Media Services](https://docs.microsoft.com/en-us/azure/media-services/latest/create-account-howto) account. During the creation of the Logic App flow we also need to specify an Azure Log Analytics Workspace. It is best you already set one up now using these simple steps: [Quick Create Workspace](https://docs.microsoft.com/en-us/azure/azure-monitor/learn/quick-create-workspace)

## prerequisites:
- Azure Subscription
- AMS account created
- Log Analytics Workspace
