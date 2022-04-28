# Get-Current-SCOM-Notification-Server

The SCOM Management Server hosting object "Alert Notification subscription Server" is the current Notification Server, which will make SMTP connection (SMTP channel), or executing Command (Command channel). However the property of this object (such as [Microsoft.SystemCenter.AlertNotificationSubscriptionServer].PrincipalName]) seems not updated even when the object is hosted on another SCOM management server. 

This script is using SCOM HealthService Task "Show Running Rules and Monitors for this Health Service" to identify which Management Server is actually hosting this "Alert Notification subscription Server" object, and display the management server name. 
