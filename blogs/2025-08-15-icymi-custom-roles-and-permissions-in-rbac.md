---
title: 'ICYMI: Custom Roles and Permissions in RBAC'
url: https://firehydrant.com/changelog/icymi-custom-roles-and-permissions-in-rbac/
date: '2025-08-15'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters! We've got some exciting updates to share with you this week, including powerful new RBAC capabilities and several quality-of-life improvements that'll make your incident management smoother than ever.

🔐  RBAC Custom Roles

Create roles that match your organization's unique structure.

We're thrilled to introduce Custom Roles in FireHydrant! Now you can create permission sets that perfectly align with how your teams actually work. Whether you need read-only observers, incident commanders with full control, or something in between, custom roles let you define exactly who can do what.

🔑 Key Features

Build Your Own Roles: Start from scratch or modify our pre-built templates. Create roles like "Weekend On-Call Engineer," "Incident Observer," "Retrospective Lead," or whatever makes sense for your organization.

Granular Permissions: Mix and match permissions across every area of FireHydrant:

Incidents (view, create, modify, resolve)

Runbooks (execute, edit, create)

Retrospectives (view, edit, publish)

Service Catalog (manage services, environments, functionalities)

Integrations and more!

Team-Specific Assignment: Assign custom roles at the team level. Engineers on Team A can have different permissions than Team B, ensuring everyone has access to exactly what they need.

System Roles to Get Started: Don't want to start from scratch? You can copy an existing system provided role and customize it to fit your needs.

What does this mean for you?

Perfect Fit: No more workarounds or overly broad permissions - create roles that match your actual job functions

Faster Onboarding: New hires get exactly the right permissions from day one

Better Security: Limit access to sensitive areas while still empowering teams to respond quickly

Evolve Over Time: Easily adjust roles as your organization grows and changes

🚀 Available Now: Organization owners can create and manage custom roles in Settings → Roles & Permissions. Check out our blog post and documentation to learn more!

🐛 Bug Fixes & 💅Improvements

But that’s not all we’ve done this week. Here’s a healthy shipment of all of the bug fixes and improvements we have delivered to make your experience more reliable and intuitive.

🔥Incident Management Enhancements

Fixed File Upload Issues: We squashed a bug that was causing silent failures when uploading images with special characters in filenames. Mac screenshots with those pesky unicode characters? No problem now!

Scrollable Responder Lists: Teams with 10+ members can now properly scroll through the add responders menu instead of having names cut off. Because nobody should be left out of an incident response!

Timezone-Friendly Date Pickers: Fixed multiple timezone-related issues in audit logs and analytics:

Users in forward timezones can now select "today" without it jumping to yesterday

Future date selections now gracefully adjust to current time instead of showing errors

Late-night date range selections work as expected

Smarter Runbook Tracking: Runbooks now display when they were last executed and which incident they were used for, replacing the previous "Last Updated" column with more actionable "Last Executed" information. Hover over the incident reference to see full details without leaving the page!

Required Fields in Retrospective Templates: Now you can set specific fields within your retrospective document as required before transitioning to a milestone.

📆 On-Call & Scheduling Improvements

Better Unclaimed Shifts Display: The unclaimed shifts section now correctly shows all coverage requests and unclaimed shifts within your calendar view range.

Visual Calendar Fixes: Removed unnecessary padding between shifts that was causing short shifts to appear as thin lines. Now even 1-hour shifts are clearly visible!

Team Schedule Persistence: Fixed a sneaky bug where adding a new user to a team would make Signals schedules disappear. Your schedules now stay put when team membership changes!

📱Slack Integration Updates

Smarter Org Switching: When using /fh switch org outside of a channel, FireHydrant now messages you directly instead of leaving you hanging. No more wondering if the command worked!

📓Status Page Improvements

Accurate Maintenance Notifications: Fixed incorrect time displays in scheduled maintenance emails. Your stakeholders will now see the correct start times for planned maintenance windows.

⚙️Integration Reliability

Multi-Jira Instance Support: Organizations with multiple Jira Cloud installations can now reliably import follow-ups from URLs, even when tickets exist in non-default projects. No more "sync pending" limbo!

💅 UI/UX Polish

We've been fine-tuning the details based on your feedback:

Escalation Policy Forms: The first step duration selector is now properly disabled to prevent confusion

Milestone Menus: Added max height with scrolling for better usability

Schedule Views: Current/next rotation information now displays correctly in team schedule tabs

User Profiles: Updated layout to match our latest design system

Coverage Requests: Significantly improved slot calculations for more accurate availability displays

🏝️ And One More Thing...

Not on call? We've replaced that boring stack of papers with a lovely island scene. Because when you're off duty, you deserve to think about beaches, not incidents! 🏖️

That's all for this week! As always, if you have any questions or feedback, our team is here to help. Stay safe out there, firefighters! 🚒
