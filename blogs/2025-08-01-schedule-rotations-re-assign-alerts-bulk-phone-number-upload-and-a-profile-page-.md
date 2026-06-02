---
title: Schedule Rotations, Re-assign Alerts, Bulk Phone Number Upload, and a Profile
  Page Redesign
url: https://firehydrant.com/changelog/schedule-rotations-re-assign-alerts-bulk-phone-number-upload-and-a-profile-page-redesign/
date: '2025-08-01'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 We've been busy! We've got four more major improvements to Signals that we shipped for you this week!

🗓️ Schedule Rotations

When coverage gets complicated, Schedule Rotations keeps it simple. We've completely reimagined how on-call scheduling works in Signals with a powerful new feature that lets you define multiple, separate rotations inside a single schedule.

What's new:

Multiple rotations per schedule: Each rotation can have its own people, timeframes, and handoff cadences - whatever your team needs to stay covered

Follow-the-sun coverage: Build seamless coverage across multiple time zones with dedicated rotations for each region

Business hours flexibility: Split shifts between business hours and overnight with separate rotation configurations

Shadow rotations: Add new hires or observers without putting them in the hot seat - they can learn without being the primary responder

Alert all active users: Configure alerts to reach everyone currently on duty across all rotations in a schedule

Complete setup overhaul: Configure everything in one streamlined screen with live preview so you know everything's right before it goes live

This isn't just an incremental update - it's a complete rethinking of on-call scheduling that makes complex coverage scenarios simple to set up and manage. Read more on our blog post about rotations: “Introducing Schedule Rotations: One Schedule, Many Rotations, Total Coverage”

🚀 Reassign Alerts



We've completely redesigned how you escalate alerts, giving you more control and flexibility in your incident response workflow. Now you have powerful options to ensure the right people respond to critical alerts, no matter how complex your team structure.

What's new:

Smart escalation dropdown: Two clear options appear directly on your alerts - "Escalate to next member" follows your existing escalation policy automatically, or "Handoff to another user" gives you full control over who takes ownership

Intuitive escalation modal: The new escalation interface provides a better user experience for selecting targets, with clear options and easy navigation

Complete audit trail: All escalation and reassignment actions are now tracked in the alert timeline with full details, so you can see exactly how alerts moved through your team

Slack integration: You can now reassign alerts directly from Slack using the new REASSIGN action option, keeping your workflow seamless

This update transforms alert escalation from a rigid process into a flexible, user-friendly system that adapts to your team's real-world needs.

☎️ Bulk Phone Number Imports

Managing contact information for large teams just became effortless! Administrators can now upload hundreds of user phone numbers in seconds using a simple CSV file or within their SCIM provisioning configuration, eliminating hours of manual data entry and reducing the risk of errors.

What's new:

CSV upload interface: Upload phone numbers for multiple users simultaneously with drag-and-drop functionality

SCIM support Add phone numbers to your user definitions and seamlessly apply them to your account with your SCIM integration

Comprehensive feedback: Detailed results showing successful updates, failed records with specific error messages, and skipped data

Template download: Get started quickly with a pre-formatted CSV template

Complete audit trail: All phone number updates are logged for compliance and tracking

This feature transforms user management from a tedious manual task into a streamlined operation that grows with your organization.

🧑‍💻 Redesigned User Profile Page

We've completely overhauled the account settings interface with a cleaner, more intuitive design that makes managing your profile and notification preferences effortless.

Two-column layout: Core profile info on the left, notifications and linked accounts in tabbed interface on the right

Inline editing: Edit your avatar, name, and contact info directly without extra navigation

Notification policy compliance: Visual indicators and one-click "Match & update all" button for policy requirements

Mobile optimization: Fully responsive design that works seamlessly on all devices

Unified contact management: All email, phone, and alternative contact methods in one place

Additionally, we've added the ability to quickly match your personal notification preferences to the global notification policy set by your organization. Either take action on each notification preference, or choose to match and update all. Getting into compliance has never been easier!

💅 Improvements

Faster On-Call Schedule Loading Eliminated 504 timeouts for teams with many on-call schedules by optimizing how we fetch shift data. API calls now only fetch data for the visible date range, significantly improving page loads for teams with 19+ schedules and preventing unnecessary server load.

Custom Event Sources Payload Limits Added clear messaging about the 16KB payload size limit for custom event sources, helping you stay within system constraints when building custom integrations.

UI/UX Polish: fixed height issues in rotation start time fields, improved month views to use weeks rather than days for better time visualization, enhanced error messaging for private incidents with more actionable guidance, and clearer shift coverage modal design showing your shift times vs. requested coverage times.

🐛 Bug Fixes

Status Page Updates Now Propagate Correctly Fixed a long-standing bug that prevented edits to status page updates from propagating through to the status pages themselves. The issue affected most note records created as part of bulk updates (when changing incident milestones, updating impacted infrastructure, etc.). When you update a status page note from the incident command center, those changes will now actually appear on your status pages.

That's all for this update! As always, if you have any questions or feedback, our team is here to help. 🔥
