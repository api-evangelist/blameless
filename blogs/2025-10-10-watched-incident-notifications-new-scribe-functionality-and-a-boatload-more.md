---
title: Watched Incident Notifications, New Scribe Functionality, and a Boatload More
url: https://firehydrant.com/changelog/watched-incident-notifications-new-scribe-functionality-and-a-boatload-more/
date: '2025-10-10'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters!🧑‍🚒 Go make some coffee, we’ve got a long changelog this week! We've been heads down the last few weeks working on high-quality bug fixes and improvements. Here's what we’ve shipped for you!

📧 Watched Incident Notifications

Never miss updates on the incidents that matter most to you. You can now subscribe to your saved incident views and get automatic notifications when matching incidents are created or updated.

What does this mean for you?

Automatic monitoring: Set it and forget it — get notified when incidents matching your saved filters pop up

Personalized alerts: Track incidents by severity, team, service, or any combination of criteria that matters to you

Better visibility: Stay informed about critical incidents without constantly checking the dashboard

Look for the bell icon next to subscribed searches in your saved search dropdown — we've streamlined the UI to make it clearer which views you're following.

Learn more about Auto-watching incidents here!

🎯 Audience-Specific Automated Updates

Want to send tailored communications to different stakeholders automatically? You can now use Audience AI Summaries as conditions in your Runbook steps! This means you can trigger emails and other communications with audience-specific summaries based on any combination of conditions you set up. Perfect for keeping executives, support teams, and engineers in the loop with exactly the info they need.

🤖 Scribe Just Got Smarter

Scribe can now join existing conference bridges directly from Slack using /fh scribe! No need to start a new bridge just to get AI-powered summaries and transcripts. If you have transcriptions enabled, Scribe can even provide a summary of the most recent conversation from the call. Plus, we've expanded Scribe's integration capabilities — you can now add Scribe to bridges created through Runbook steps, even if you're using a chat solution other than Slack.

⚙️ Microsoft Entra ID: Manage Teams with SCIM Groups

If you're using Microsoft Entra ID for identity management, you can now sync and manage FireHydrant Teams directly through SCIM groups. This integration automatically creates and updates Teams and manages member assignments based on your Entra ID groups, keeping your team structure in sync across platforms.

🏗️ Terraform Provider Updates

We've expanded our Terraform provider with several new capabilities to help you manage FireHydrant infrastructure as code:

Incident Types: Added firehydrant_incident_type as both a resource and data source

Custom Event Sources: Full support for creating and managing custom event sources (relay transposers)

On-Call Schedule Import: Import existing on-call schedules and rotations via the terraform import command

Team Memberships: New data source for team membership information

Custom Event Source Outputs: The ingest_url is now available as an output for custom event sources

💅 Improvements

Improved Alert Visibility: Signals alert descriptions containing HTML content (from integrations like Dynatrace) now render properly instead of showing raw HTML tags or stripped formatting.

More Customization: Custom text fields can now hold up to 1,000 characters, giving you more room for detailed information.

Confluence Permissions: Users with manage_integrations permission can now authorize the Confluence integration.

Google Docs Export: Rich text formatting in Retrospectives now exports correctly to Google Docs, preserving your careful formatting work.

🐛 Bug Fixes

Fixed a redirect loop that could log you out immediately after logging in when visiting the login page directly.

Resolved phone number removal issues when using SCIM provisioning.

Non-default organizations can now install the Zoom integration without issues.

Bots can now create private incidents as expected in our authorization system.

Fixed a crash that occurred when changing dropdown values in Runbook steps for integrations with boolean options (like Webex).

Resolved an issue preventing some analytics reports from exporting to CSV.

Fixed a bug that caused user names to overflow onto next column in incident transcripts

Resolved an issue causing team names to not load for incident types in the incident declaration and incident type configuration.

That's all for this week! As always, if you have any questions or feedback, our team is here to help.
