---
title: We’ve got some small but mighty improvements this week!
url: https://firehydrant.com/changelog/weve-got-some-small-but-mighty-improvements-this-week/
date: '2025-06-20'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 Here's what's shipped for you this week!

💅 Improvements

Timeline View Now Default for On-Call Schedules: We've reordered the calendar view options and made timeline view the default view for on-call schedules. This gives you a clearer, more intuitive way to see your on-call schedule at a glance.

Enhanced Table Filtering: You can now select multiple filter options simultaneously! For example, you can select both "Open" and "Acked" alert filters to see items matching either status.

Better Nested Audit Event Support: We've improved the UI to support viewing and filtering nested audit events, particularly for shift generation. This provides better visibility into complex on-call schedule changes and how they relate to each other.

Markdown Table Support: Tables in markdown are now supported across the platform, giving you more formatting options for documentation and incident updates.

Public API Access to Audit Events: Audit event data is now available through our public API. See the documentation for details.

Easier Field Removal from Incident Types: You can now easily remove fields from incident types using the trash can icon that appears when hovering over fields. Removed fields will properly disappear after saving. Simply hover over any field to see and use the removal option.

Organization Switcher on Mobile: The organization switcher is now available on mobile and tablet devices! You can change which organization you're viewing from any device, not just desktop.

🐛 Bug Fixes

Regex Validation Improvements: Updated regex validation in conditions menu so you get proper validation feedback when entering regex patterns.

Tooltip Positioning: Fixed incorrectly positioned tooltips to ensure they remain visible and properly aligned.

Form Error Scrolling: The "scroll to first error" feature now works correctly with select inputs.

Slack Channel Messaging: Improved how we handle alternative host messages - now sending a single failure message to channels while whispering directly to users for subsequent failures.

Enhanced Custom Field Filtering: Custom field option filtering now works reliably when typing filter values.

Fixed Handoff Command Issues: Fixed a bug that prevented role handoffs when assigning a role to a user who already had that role. The handoff command now works consistently in all scenarios.

That's all for this week! As always, if you have any questions or feedback, our team is here to help. 🔥
