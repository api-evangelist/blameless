---
title: Enhanced Alert Management & Filtering, Automatic Zoom Transcriptions and More
url: https://firehydrant.com/changelog/enhanced-alert-management-and-filtering-automatic-zoom-transcriptions-and-more/
date: '2025-10-23'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒We know that many of you have had a busy week! (Check out our post-incident write-up from Monday’s AWS outage here.) So take a break, and check out what we’ve shipped for you over the past few weeks!

🎯 Enhanced Alert Management & Filtering

We've overhauled our tables with three major improvements that ship to the Alerts list. You now get a date/time range picker for filtering by time windows, dynamic pagination with per-page configuration, and a redesigned search and filter layout. This gives you better control over sifting through high-volume alert data.

We also added a "My Teams" quick filter button to instantly surface alerts scoped to your team membership.

🤖 Automatic Zoom Transcription

Added support for Zoom's automatic AI scribe behavior, where bots start recording on meeting entry without needing host intervention. You can toggle this per Runbook step, and we'll post a notice to the incident's Slack channel when automatic recording begins.

💅 Improvements

Continue Posting Status Updates Post-Resolution – We enabled status update notifications to continue posting to Slack, Microsoft Teams, and Status Pages after incident resolution.

Better Loading Indicators in Timeline – Improved loading states for long lists across the application.

Improved Member Table Layout – Added max widths and tooltips to prevent table overflow on long names or display values, keeping the member table readable at a glance.

/fh edit Command Field Preservation – The /fh edit Slack command now respects existing field values and supports custom fields, so you're not starting from a blank slate each time.

Webhook Endpoint Field Simplification – Changed the webhook endpoint field from a liquid-enabled input to a regular text field. This prevents confusion about multi-destination routing capabilities that don't exist.

Integrations Page Default Tab – Set the Integrations page to default to the "All" tab, and we now persist your last tab selection in local storage so you return to your preferred view.

Voice Paging Error Details – Improved voice call escalation error messages to return specific failure reasons (e.g., "alert already acknowledged", "no further escalation available") instead of generic error text.

🐛 Bug Fixes

Slack Attachments in RBAC-Enabled Orgs – Fixed a bug where attachments posted by non-FireHydrant users in Slack incident channels weren't appearing in the timeline for organizations with RBAC enabled. Now images and attachments surface correctly regardless of poster role.

Custom Date/Time Fields in Alert Routing – Unblocked custom date/time fields in alert routing configuration, allowing more precise rule definitions.

Severity Creation Validation – Fixed a crash that occurred when submitting a severity without selecting a type. The form now properly enforces the required severity_type field.

Milestone Field Validation on Resolution – Tightened validation in the Incident form to require all milestone timestamps be filled before marking an incident resolved, preventing incomplete incident data.

Analytics Table Filtering – Fixed incorrect incident filtering in the catalog analytics views to ensure tables display the expected result set.

PDF Export Image Handling – The PDF export now handles images better. We respect the image size and wide header logos now don't overlap the company name.

As always, if you have any questions or feedback, our team is here to help! 🔥
