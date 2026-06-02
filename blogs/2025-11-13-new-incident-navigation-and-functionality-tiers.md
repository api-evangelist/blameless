---
title: New Incident Navigation and Functionality Tiers
url: https://firehydrant.com/changelog/new-incident-navigation-and-functionality-tiers/
date: '2025-11-13'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 Here's what we’ve shipped recently!

Refreshed Incident Page with Tab Navigation

We're rolling out a cleaner, more intuitive Incident page with new tab navigation to easily switch between Incident Details and Retrospectives. The refreshed header design now features action buttons that update based on which tab you're viewing — giving you exactly what you need, right when you need it. All of your existing functionality works just as before, just with a smoother, easier-to-navigate experience.

Functionality Tiers for Smarter Automation

Functionalities can now be assigned tiers (0-5) to indicate their importance, just like services. This gives you powerful new automation capabilities: set runbook conditions based on functionality criticality to automatically attach or execute specific steps depending on what's impacted. For example, tier the payment processing functionality as tier 5, and automatically escalate to your payments team and trigger a dedicated runbook when it goes down. Or keep lower-tier features at tier 1 and run lighter workflows. You control the response based on what matters most to your business.

Improvements 💅

Conference Bridge Links in Slack We've added back conference bridge links directly to your Slack messages — both in incident linkbacks and alert notifications. Now your team can jump into the right meeting with one click, without hunting through messages for connection details.

Microsoft Teams Group Chat Improvements When a functionality or service is assigned to an incident, team members are now automatically added to the incident MS Teams group chat. This works for both direct service assignments and when adding FireHydrant Teams as responders, keeping everyone in sync from the start.

Filter Incidents by Attached Runbooks: Find incidents faster with a new filter that lets you search by attached runbooks.

Post-Resolution Updates Now Persist: Fixed a bug where status updates posted via Slack stopped appearing in integration channels after resolution. Updates now continue flowing through Slack, Microsoft Teams, and Status Pages throughout the entire incident lifecycle.

Better Milestone Date Validation: The milestone form now validates dates with clear error messages (MM/DD/YYYY format) and prevents invalid dates that caused metrics failures. 

Valid dates range from 01/01/2000 to one year in the future.

Improved Time Selector Layout: Fixed overlapping buttons in the milestone time form that were covering the actual time display. Your forms should look much cleaner now.

Markdown Fields Export Properly: Markdown and Instructional Text fields in your templates now export correctly to both Confluence and Google Docs.

Lifecycle Milestones in Default Templates: We've updated default retrospective and incident templates to use lifecycle_milestones, giving you access to milestone names. If you're using custom templates, you may need to update them to leverage this new capability or re-add your Export steps to runbooks.

GIF Handling in PDF Exports: Fixed an error that prevented PDFs from rendering or downloading when they contained GIFs.

Confluence Image Export Fixed: Retrospectives with images now export to Confluence without errors.

Bug Fixes 🐛

Effective At Settings Now Work Correctly: Fixed a bug where the "Effective At" setting wasn't being applied when adding or updating responders. Now your responders are assigned exactly when you specify — immediately, at next handoff, or on a custom date.

Coverage Gap Notification Interval Persists: Fixed a bug where the Coverage Gap Notification Interval would always revert to "1 week" after saving. You can now keep it set to "1 day", "2 weeks", "1 month", or any other value you choose.

Slack Notification Preferences Dropdown: Fixed a dropdown that was being cut off in the Slack channel notification preferences table.

Edit Message Crash Resolved: Fixed a crash that occurred when clicking "Edit message" on incident timeline events that don't support editing.

Timezone Handling in Alert Filtering: Fixed date range filter timezone handling to send local timezone information to the API. The date picker now correctly preserves your selected local time instead of converting to UTC, ensuring alerts aren't accidentally excluded from filter results.
