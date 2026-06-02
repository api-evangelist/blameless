---
title: Mobile App Reliability, Web App Improvements, and Year-End Polish
url: https://firehydrant.com/changelog/mobile-app-reliability-web-app-improvements-and-year-end-polish/
date: '2025-12-12'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 As we wrap up 2025, we're polishing things up and squashing bugs!

📱 Mobile App Stability Improvements

We've been hard at work making the mobile app more reliable:

Android Login Fixed: Resolved a crash during login on Android caused by callback URLs being incorrectly parsed as deep links.

Push Notifications Now Work from Cold Start: Fixed an issue where tapping a push notification when the app was completely closed would open the app but fail to navigate to the correct alert. Now you'll land exactly where you need to be.

More Resilient Push Notification Registration: Fixed a crash during push notification registration that could occur when handling duplicate device name conflicts.

💅 Improvements

Consistent Filtering Across Runbooks: The Runbook tab in incidents now includes the same search and filter capabilities you're familiar with throughout the rest of FireHydrant. Quickly find and filter for specific runbooks without switching contexts.

More Milestone Options in Runbook Steps: The milestone dropdown in the "Update Incident Details" runbook step now includes milestones from the "Started" lifecycle phase (like "Detected"). This gives you more flexibility in tracking incident progress through your runbook automation.

Clearer Ticket Update Labels: Ticket updates in the incident timeline now display human-readable labels, making it easier to understand what happened at a glance (e.g., "Created ticket" instead of cryptic system codes).

More Accurate User Involvement Time Tracking: The system now uses session-based tracking that better reflects actual engagement time versus elapsed time, giving you more accurate responder metrics in analytics.

🐛 Bug Fixes

Runbook Step Repeat Durations Now Stick: Fixed a frustrating bug where runbook step repeat durations were unexpectedly resetting to 5 minutes when editing steps, even when you had configured longer intervals (like 2 hours). Your repeat duration settings now correctly preserve existing values.

That's all for this week! As always, if you have any questions or feedback, our team is here to help.
