---
title: Additional RBAC For Incident Types and Severities; No Tricks, All Treats
url: https://firehydrant.com/changelog/additional-rbac-for-incident-types-and-severities-no-tricks-all-treats/
date: '2025-10-31'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
👻 This Halloween we’ve opted out of tricks so we’re shipping a some serious treats! Here's what's new this week, firefighters 🧑‍🚒!

🔐 Role-Based Access Control for Incident Types and Severities

There’s nothing scarier than a SEV0. Now you can take control of incident creation across your organization by restricting both incident types and severities based on user roles, ensuring the right people have access to the right tools.

Restrict Incident Types by Role Organizations can now control which incident types users are allowed to create based on their role. Admins configure permissions in Settings → Incident Types, and users only see the incident types they're authorized to use.

Restrict Severities by Role You can also restrict which severities users can declare when creating incidents. Prevent junior team members from accidentally declaring SEV1s, align severity selection with your organizational escalation policies, and maintain consistency across teams with different responsibilities.

🤖 Enhanced Audience Controls

You now have more granular control over AI-powered incident summaries. Admins can configure which data gets submitted for summarization on a per-audience basis—set it during audience creation or adjust it anytime in your audience settings. This means each stakeholder group gets summaries tailored to exactly the information they need.

💅 Improvements & Enhancements

Better Alert Tag Visibility in Slack — We're giving you more control over Signals alert tags in Slack. Previously, tag filters were required to show any tags at all, and we'd only show the first 6. Now, all of your alert's tags will display in Slack messages — with tag filters being completely optional.

Clearer Incident Field Configuration — We've made the incident types form more intuitive. Removed the confusing drag-to-reorder interaction since fields can't actually be reordered, added helpful tooltips for non-editable fields, and now you'll see a warning before saving if any fields won't be included because they're missing required values.

More Flexible Field Requirements — Globally visible fields can now be marked as required, and if you have fields already required at a specific milestone, you can now change them to any earlier milestone. More flexibility in how you structure your incident data.

Visibility into Milestone Changes — Milestone timestamp edits now appear as timeline events, so you can see exactly which milestones were adjusted and when — giving you full visibility into incident timing changes made during or after resolution.

Better Image Handling in Retrospectives — Retrospectives now handle images the way you'd expect. Copy and paste GIFs, drag and drop multiple files, and work with images seamlessly as you document what happened and what you learned.

Improved Table Display — Fixed table rendering to properly wrap long content, making your data easier to read and reducing unnecessary horizontal scrolling.

Incident Channel Privacy Control — For Enterprise Grid organizations with the right permissions, incident channels can now be automatically converted from public to private — giving you tighter control over who sees sensitive incident details.

🐛 Bug Fixes

Signals Alerts Filtering — Fixed the /fh alerts Slack command to show only Signals alerts instead of pulling in alerts from every integration (PagerDuty, OpsGenie, etc.), keeping your Slack feeds clean and consistent with your web UI.

Dashboard Alert Filtering — Fixed the Dashboard's "All Alerts" Kanban board incorrectly displaying Jira tickets and other non-Signals alerts. Now it properly filters to Signals alerts only.

Mobile Alert Navigation — Fixed alert notifications on mobile not navigating to the correct screen. Tapping an alert notification now reliably takes you to alert details instead of leaving you on the dashboard.

That's all for this week! As always, if you have any questions or feedback, our team is here to help. Happy Trick-or-Treating!
