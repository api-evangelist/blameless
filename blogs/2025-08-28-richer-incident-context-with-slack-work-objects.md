---
title: Richer Incident Context with Slack Work Objects
url: https://firehydrant.com/changelog/richer-incident-context-with-slack-work-objects/
date: '2025-08-28'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 We've got some exciting updates to share with you this week!

🔗 Enhanced Slack Integration with Work Objects

Richer details and interactions now live directly in Slack - no more context switching.

We've integrated with Slack's new Work Objects functionality to bring richer, more interactive incident information directly into your Slack channels. When you share FireHydrant incident links, Slack now automatically expands them with live, interactive context.

What does this mean for you?

Rich incident previews: See severity, status, roles, and key details right in the unfurl

Real-time updates: Incident flexpanes update automatically as your incident evolves

Quick updates: Update specific incident details directly from Slack without jumping to the web UI

This integration transforms how your team experiences incidents in Slack making every incident link a window into your response efforts.

Note: Slack has begun to roll out Work Objects, but it may not be available to all Slack customers yet. We expect everyone to have the new experience by the end of September.

🗂️ Message Retention Policies for Slack & MS Teams

Control how long your messages are kept with new retention policies for chat messages. You can now configure how long FireHydrant retains messages from your Slack and Microsoft Teams incident channels.

Key features:

Set custom retention periods per integration

Automatically clean up old incident messages

Permanent deletion of messages past retention policy

Maintain compliance with your data retention policies

Configure directly from your integration settings

You can configure your message retention policies directly from your integrations configuration settings within the WebUI. Navigate to Settings -> Integrations and edit your Slack or MS Teams integrations to get set up!

🐛 Bug Fixes

Team assignment for impacted services: We squashed a bug that sometimes prevented all responding teams from being alerted or assigned to your incidents when marking a service or functionality as impacted

Email display in members table: Long email addresses no longer overflow into adjacent columns now truncating cleanly with tooltips for full viewing

Audit log formatting: Names in the audit log table now truncate properly instead of overlapping with dates

Navigation prompts: Fixed unnecessary "unsaved changes" warnings when navigating away from email destination pages in event sources

SSO navigation: When SSO isn't configured yet, we now disable the nav option with a helpful tooltip instead of redirecting you away

That's all for this week! As always, if you have any questions or feedback, our team is here to help. Keep fighting those fires! 🔥
