---
title: 'Introducing: FireHydrant MCP Server'
url: https://firehydrant.com/changelog/introducing-firehydrant-mcp-server/
date: '2025-07-18'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 Here's what's shipped for you this week!

🧪 MCP Server Now Available in Beta!

We're excited to announce the beta release of our Model Context Protocol (MCP) server! This new integration allows AI assistants like Claude to directly access your FireHydrant data and perform incident management tasks through natural language.

What can you do with MCP?

Query incident data and metrics conversationally

Get real-time status updates on ongoing incidents

Access your service catalog and on-call schedules

Generate reports and analytics through AI assistance

Ready to try it? The MCP server beta is available now for all customers. Check it out here! https://www.npmjs.com/package/firehydrant-mcp

📝 Custom Field Updates in Runbooks

We've added a powerful new Runbook step that lets you update incident custom fields automatically! This new step supports all types of custom fields, giving you complete control over your incident data as your response progresses.

What does this mean for you?

Automate field updates based on incident progression

Keep custom data consistent across your workflow

Less manual data entry, more time fighting fires

🤖 AI Summary Condition Triggers

Now you can create Runbook conditions that trigger when AI summaries are generated or updated! Set up automatic notifications via email, Slack, or other channels whenever your incident summaries change.

Perfect for:

Keeping stakeholders updated with the latest AI-generated insights

Triggering follow-up actions when summaries are refreshed

Automating communication workflows around incident analysis

💅 Improvements

Mark Alerts as "Noise": Our mobile app now lets you mark alerts as "Noise" directly from your phone! Reduce alert fatigue by quickly identifying and filtering out non-actionable alerts while on the go.

Timeline View Customization We’ve added configurable duration options to the on-call timeline view. Now you can set the time window to see exactly what you’re looking for.

Mobile App Logout Confirmation: Added a confirmation dialog when logging out of the mobile app to prevent accidental logouts. Because nobody wants to accidentally log out when they're trying to respond to an incident!

Slack Guest Access for On-Call: Slack guests can now view on-call schedules! When users aren't linked to FireHydrant from Slack, they can enable or disable access to /fh oncall commands, making it easier for external collaborators to stay informed.

Jira Integration Enhancements: We’ve added a manual sync button for Jira Cloud and Jira On-Prem integrations so you can refresh your connection whenever needed. New ticketing projects now automatically get default field mappings to streamline your setup.

ServiceNow Health Monitoring: Added integration status warnings if your ServiceNow field mappings aren't properly configured, helping you catch setup issues before they impact your workflow.

Enhanced iCal Details: Improved shift change details in iCal exports with better timestamps and change tracking, so your calendar always reflects the most current schedule information.

Organization Context Protection: Added a helpful modal that appears when users try to interact with alerts from a different organization context, preventing confusion and ensuring you're always working in the right space.

Optimized Real-Time Updates: Introduced a centralized incident channel provider that manages Pusher subscriptions more efficiently, eliminating race conditions and reducing unnecessary network traffic for faster, more reliable real-time updates.





That's all for this week! As always, if you have any questions or feedback, our team is here to help. Keep fighting those fires! 🔥
