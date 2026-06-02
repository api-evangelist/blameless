---
title: Mobile App Updates, Better Integration Performance, and UX Improvements
url: https://firehydrant.com/changelog/mobile-app-updates-better-integration-performance-and-ux-improvements/
date: '2025-07-11'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 Here's what shipped for you this week!

📱 Mobile App Improvements

We've made significant improvements to how you navigate and interact with alerts across the platform:

Noisy Alert Support: Now you can take advantage of our Alert Noise feature from within the mobile app! Updates include dedicated actions, UI controls, and improved status display.

Direct Communication Channel Links: You can now directly open Slack and Microsoft Teams channels from the Related Incidents section, making it easier to jump into ongoing conversations without hunting for the right channel.

Better Back Button Behavior: When viewing an alert from the Home screen or Alerts screen, the back button now correctly returns you to your originating screen instead of following the navigation stack history. No more getting lost in the navigation flow!

Stabilized Alert Timeline: The alert timeline component no longer re-renders unnecessarily when other parts of the alert screen update, providing a smoother and more stable viewing experience.

Better Tag Display: Tags in alert details now properly wrap instead of truncating, so you can see all your tag information without navigating out of the mobile app.

💅 Improvements

Optimized Microsoft Teams Integration: We've updated the Microsoft Teams integration to request more specific and organized permissions when users connect their Teams accounts to FireHydrant. Since we're reducing permissions rather than adding new ones, existing authorizations should continue to work without requiring re-authorization. To opt in for the new permissions scope you can re-authorize your installed FireHydrant app.

Smarter Jira Performance: Replaced expensive live API calls to Atlassian with cached data from our database for issue types and field mapping. This significantly reduces load times and improves reliability when configuring Jira integrations.

🐛 Bug Fixes

Improved Schedule Selector: Long schedule names are now properly truncated in the schedule list, preventing UI overflow and making the interface cleaner.

Smarter Notifications: We now skip handoff notifications for shifts that belong to deleted on-call schedules or rotations, preventing confusing notifications for non-existent schedules.

Design Consistency: Fixed several minor design issues including sentence case policy compliance, header sizes in Command Center tabs, and alignment issues in the teams page.

Line Break Support: Task descriptions now support line breaks for better formatting, and we've fixed an issue where the task list wouldn't refresh when new tasks or lists were added.

ServiceNow Integration Fixes:

Services can now be properly "un-discarded" when ServiceNow CMDB records sync back into the FireHydrant Catalog.

Removed erroneous milestone mapping code that was throwing errors

Cleaned up the inbound field mapping interface to remove the unused "Current milestone" option.

That's all for this week! As always, if you have any questions or feedback, our team is here to help. 🔥
