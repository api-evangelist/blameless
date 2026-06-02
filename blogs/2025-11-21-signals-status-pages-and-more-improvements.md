---
title: Signals, Status Pages & More Improvements
url: https://firehydrant.com/changelog/signals-status-pages-and-more-improvements/
date: '2025-11-21'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
Hey there, firefighters 🧑‍🚒 We've been busy squashing bugs and polishing the experience this week!

Signals Improvements

On-call schedule timeline view zoom controls: We've added inline zoom controls to the timeline view, making it way easier to adjust your time range and actually click on those super short shifts (we're looking at you, 30-minute coverage blocks). No more fumbling around trying to select tiny shift cards.

Clearer alert targeting: The alert timeline now clearly shows when alerts are directly targeted to specific teams, escalation policies, schedules, or users. Even better, everything's clickable so you can quickly jump to the targeted resource. Less guessing, more doing.

Status Page Improvements

Markdown formatting in emails: Status page update emails now properly render markdown formatting including bold text, lists, headers, and links. Previously all that formatting showed up as plain text, which... wasn't great.

Delete status page updates: You can now delete status page updates directly from incidents. A delete button appears next to each update for owners with manage_incidents permission. Note: Updates from Statuspage.io can't be deleted due to integration limitations.

💅 Other Improvements

Better form validation: Fixed a sneaky bug where required fields (description, severity, priority, impacts, teams, tags, and milestones) weren't being validated on incident declaration forms. Now you'll actually see validation errors instead of mysteriously losing your data.

Correct Opsgenie paging priority: When you create a page via /fh page, the incident's priority is now automatically pre-selected. No more P1 incidents accidentally sending P3 alerts.

Fixed CSV exports: CSV download links in incident and user export emails now properly download instead of opening as plaintext pages in your browser.

Partial shift button clarity: Changed the button copy when claiming a partial shift to be less confusing.

Runbooks table resizing: The runbooks table no longer overflows the page or loses columns when you resize your window.

Terraform provider updates: Fixed inbound email resource configuration, added support for custom milestone resources and lifecycle phase data sources, and migrated functionalities, team management, and catalog entry resources to the latest SDK.

🐛 Bug Fixes

Retrospective PDF exports now include the alerts section.

Fixed extra blank space showing up after each question when exporting retrospectives to Confluence.

Fixed email notification links to account settings after we changed the URL structure.

That's it for this week! Keep the feedback coming - we're always listening.
