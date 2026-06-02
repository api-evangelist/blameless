---
title: '🧨 Fireworks Preview: Eight New Signals Features'
url: https://firehydrant.com/changelog/fireworks-preview-eight-new-signals-features/
date: '2025-07-03'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 We've shipped eight powerful new features to make your on-call experience smoother, smarter, and more collaborative! Make sure to keep scrolling to catch all of the features, improvements, and bug fixes! 

💬 Signals for Microsoft Teams

You can now directly route alerts directly to Microsoft Teams channels or direct messages in your escalation policies. Now all of your teams can receive alerts wherever they work. Microsoft Teams can now be set as a user notification preference, a target to an escalation policy, and configured as your team’s channel.

🔔 Notification Preferences Policy

Admins can now set preferred channels and delay settings for alerting notification policies for each priority level. Your users will see policy compliance status in their settings, so that they can ensure they are within the expected notification time. Admins can also view and filter the users list by those within policy and download a CSV for further processing.

📊 Team Analytics Views Revamped

We’ve updated the analytics page in the Team, Service, Functionality, and Environment pages to be more actionable from your first look. You can now see high level details of the alerts opened, acknowledged, escalated, and resolved alongside incidents declared — all with MTTA, MTTR, and noise ratio metrics in one clean view.

🤝 Handoff Summary

At the end of every shift, our Slack bot sends the incoming engineer a summary including alert + incident counts and direct links to dashboards. Click on any link to see more details within the command center. You can enable this by assigning a Slack channel to your team and using the /fh channel command to enable your team’s channel to receive notifications.

🕳️ Coverage Gap Notifications

Get daily Slack and email alerts to notify your team about coverage gaps with direct links to fix them fast. Set to notify your team at 9am in your schedule's configured timezone.

🚨 Alert Noise

Tag unnecessary alerts as noise directly from Slack threads or the FireHydrant UI. Filter them in the Alerts view and track "noise over time" trends in Analytics with full timeline context.

🔁 Alert Visualization

Now you can preview exactly how an alert will escalate through your organization. Drop in a sample payload and see exactly who gets notified, when, and how. Change the time or date to simulate different routing scenarios and catch misconfigurations before they cause problems.

🛠️ Signal Event Debugging

The new "Debug Custom Event Sources" tab shows all incoming payloads from your custom sources for the last 7 days — even failed ones. See what was accepted/rejected and get direct links to created Signals. You can now easily review any incoming payload and ensure your alerts contain all the details that your team needs.



💅 Improvements

Enhanced AI Summary Experience: Added helpful text when AI summary regeneration takes longer than expected, so you'll know the system is working and not stuck.

Improved Toggle Button States: Toggle buttons now properly track and display their active state, making it clearer when features are enabled or disabled.

Better AI Incident Descriptions: Enhanced our AI incident base prompt with improved rules for handling abbreviations, resulting in clearer and more consistent incident summaries.

Better Incident Creation Flow: When using shortcuts to open incidents, descriptions are now properly included, ensuring you don't lose important context during the creation process.

Enhanced On-Call Shift Display: The shifts section on the on-call page now focuses on what matters most - showing only unclaimed shifts and those requesting coverage, reducing noise and helping you focus on actionable items.

Streamlined Confluence Integration: Removed unnecessary space type filters from the Confluence integration, simplifying configuration and reducing confusion.

Incident Type Support for Alert Actions: You can now specify incident types when configuring alert actions, giving you more control over how alerts create and categorize incidents.

Signals Migration Tool Updates: Now when you use our signals-migrator, your rotation order will be maintained, making it that much easier to migrate your team over to Signals. 

🐛 Bug Fixes

More Reliable On-Call Sync: We fixed a bug that could prevent Slack user groups from being re-enabled during on-call syncs. Now when syncing on-call users, we properly check group status and re-enable them as needed. Plus, we've added helpful debugging messages when workspace admins need to update permissions or when users are no longer workspace members.

Better Alert Target Pagination: Fixed pagination issues for alert targets so you can now properly navigate through all your alert configurations without getting stuck.

Async User CSV Export: Fixed the user CSV export process to handle large datasets more efficiently with asynchronous processing.

Improved Field Descriptions: Fixed the display of severity descriptions and incident type field descriptions for better clarity when creating and managing incidents.

That's all for this update! As always, if you have any questions or feedback, our team is here to help. Keep fighting those fires! 🔥
