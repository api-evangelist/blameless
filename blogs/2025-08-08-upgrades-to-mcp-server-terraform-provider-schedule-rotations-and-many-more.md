---
title: Upgrades to MCP Server, Terraform Provider, Schedule Rotations, and Many More
url: https://firehydrant.com/changelog/upgrades-to-mcp-server-terraform-provider-schedule-rotations-and-many-more/
date: '2025-08-08'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 We are full steam ahead on improving the overall feel of our platform, fixing bugs, and making improvements throughout! Here's what's shipped for you this week!

🖥️ MCP Server Upgrades

One-Click FireHydrant Integration for Claude Desktop: We've packaged our Model Context Protocol (MCP) server as a Desktop Extension (.dxt file), making it incredibly easy to connect Claude Desktop with your FireHydrant organization. Desktop Extensions solve installation complexity by bundling an entire MCP server (including all dependencies) into a single installable package.

Read/Write Scope Controls: You can now specify read-only mode when using our MCP server, giving you granular control over permissions. This enhancement allows teams to provide Claude with FireHydrant access while maintaining strict security boundaries around what actions can be performed.

Improved VSCode Compatibility: We fixed validation errors that were making the MCP server unusable in VSCode by removing untyped arrays from retrospective update operations. The server now properly validates tool schemas, ensuring smooth integration with stricter MCP tool validation in development environments.

Route Name Bug Fix: We fixed a bug where some route names were too long and causing connection issues. This ensures more reliable communication between Claude and your FireHydrant organization, preventing timeouts and failed requests that could interrupt your workflow.

🏗️ Terraform Provider Support for On-Call Schedule Rotations

Infrastructure as Code for On-Call Rotations: You can now manage your complex schedules enabled by on-call schedule rotations directly through our Terraform provider! This major enhancement to our Terraform provider adds both data source and resource support for rotations, allowing you to take advantage of the full power of Schedule Rotations. If you’re not sure how to get started you can follow our guide here!

📅 On-Call Schedule Rotations Improvements

Saved Views for On-Call Schedules: We've improved how you manage your on-call schedules with persistent visibility preferences! Now when you uncheck schedules in the on-call tab, your selections stay saved across browser sessions. Each team maintains its own set of preferences, so you can focus on the schedules that matter most to your workflow.

Improved Rotation Deletion Experience: Deleting the last rotation in a schedule now works more intuitively. When you attempt to delete the final rotation, the UI clearly indicates that the entire schedule will be deleted (since schedules require at least one rotation). The confirmation dialog now properly explains what will happen, preventing confusion.

Clone Rotations to the Same Schedule: You can now clone a rotation into the same schedule. This can help users create complex schedules by copying an existing rotation configuration along with the users.

Enhanced Timeline View: We’ve reduced vertical padding in timeline views to show more schedules and rotations on screen at once.

💅 Improvements

Better Runbook Step Positioning: When retrying failed runbook steps, we now insert the retried step directly after the original one instead of appending it to the end. This ensures that follow-up steps using the "previous runbook step" operator continue to work as intended.

Rotation Selection in Call Routing: You can now select specific rotations when configuring call routing in "Direct connect" mode. When a schedule is selected, a rotation dropdown appears to let you choose the correct rotation. If there's only one rotation, it's automatically selected for you.

Enhanced Zoom Integration Management: Added a "Reauthorize" button for Zoom integrations in the Linked Accounts section, making it easier to refresh your Zoom connection when needed. We've also improved flash messages to better distinguish between initial authorization and reauthorization events.

Warning for Missing Escalation Policies: Added a helpful warning indicator in the Signals Sources page when a selected team has no default escalation policy. The warning includes a direct link to create one, helping you catch configuration issues before they impact your alerting.

Read-Only API Tokens: You can now create API tokens with read-only permissions, with options to allow reading private incident data while restricting write access.

🐛 Bug Fixes

Team Schedule Visibility: Fixed an issue where Signals schedules would disappear when adding a new user to a team.

Multi-Organization Incident Creation: We fixed a bug that made it cumbersome to declare incidents from alerts in accounts with multiple organizations. You'll now be automatically switched to the correct organization for the alert — no more need to explicitly run /fh switch org.

Slack Channel Archiving: Fixed an issue that prevented automatic archiving of incident channels in Slack workspaces where channel management is restricted to administrators. We now properly use admin user tokens when needed.

CSV Export Filtering: Resolved a bug that prevented incident CSV exports from being delivered when filtered by lifecycle phase or milestone.

Component Health Status: Fixed component health status to properly recognize when incidents have reached post-incident or closed phases, ensuring components show as operational when incidents are truly resolved.

Scheduled Maintenance Display: Prevented archived incidents from showing scheduled maintenances in the UI.

Private Incident Notifications: Stopped posting Slack messages about failed internal runbook steps when declaring private incidents. 

That's all for this week! As always, if you have any questions or feedback, our team is here to help.
